# Comparing `tmp/ethos-u-vela-3.7.0.tar.gz` & `tmp/ethos-u-vela-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/timhal01/work/mlplatform_ethos-u-vela/dist/.tmp-f8_rjh0g/ethos-u-vela-3.7.0.tar", last modified: Tue Feb 28 14:04:06 2023, max compression
+gzip compressed data, was "ethos-u-vela-3.8.0.tar", last modified: Wed May 24 15:05:53 2023, max compression
```

## Comparing `ethos-u-vela-3.7.0.tar` & `ethos-u-vela-3.8.0.tar`

### file list

```diff
@@ -1,316 +1,319 @@
-drwxr-x---   0 timhal01  (1000) timhal01  (1000)        0 2023-02-28 14:04:06.000000 ethos-u-vela-3.7.0/
--rw-r-----   0 timhal01  (1000) timhal01  (1000)       94 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/.gitignore
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1442 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/.pre-commit-config.yaml
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     3604 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/API.md
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     7261 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/BUGS.md
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2582 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/CONTRIBUTIONS.md
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     3451 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/DEBUG_DB.md
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    11357 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/LICENSE.txt
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    21340 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/OPTIONS.md
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    13043 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/PERFORMANCE.md
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    11650 2023-02-28 14:04:06.000000 ethos-u-vela-3.7.0/PKG-INFO
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     9569 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/README.md
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    12539 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/RELEASES.md
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     4507 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/SECURITY.md
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    16962 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/SUPPORTED_OPS.md
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2449 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/TESTING.md
-drwxr-x---   0 timhal01  (1000) timhal01  (1000)        0 2023-02-28 14:04:06.000000 ethos-u-vela-3.7.0/ethos_u_vela.egg-info/
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    11650 2023-02-28 14:04:05.000000 ethos-u-vela-3.7.0/ethos_u_vela.egg-info/PKG-INFO
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    10664 2023-02-28 14:04:06.000000 ethos-u-vela-3.7.0/ethos_u_vela.egg-info/SOURCES.txt
--rw-r-----   0 timhal01  (1000) timhal01  (1000)        1 2023-02-28 14:04:05.000000 ethos-u-vela-3.7.0/ethos_u_vela.egg-info/dependency_links.txt
--rw-r-----   0 timhal01  (1000) timhal01  (1000)       47 2023-02-28 14:04:05.000000 ethos-u-vela-3.7.0/ethos_u_vela.egg-info/entry_points.txt
--rw-r-----   0 timhal01  (1000) timhal01  (1000)      106 2023-02-28 14:04:05.000000 ethos-u-vela-3.7.0/ethos_u_vela.egg-info/requires.txt
--rw-r-----   0 timhal01  (1000) timhal01  (1000)        7 2023-02-28 14:04:05.000000 ethos-u-vela-3.7.0/ethos_u_vela.egg-info/top_level.txt
-drwxr-x---   0 timhal01  (1000) timhal01  (1000)        0 2023-02-28 14:04:06.000000 ethos-u-vela-3.7.0/ethosu/
-drwxr-x---   0 timhal01  (1000) timhal01  (1000)        0 2023-02-28 14:04:06.000000 ethos-u-vela-3.7.0/ethosu/config_files/
-drwxr-x---   0 timhal01  (1000) timhal01  (1000)        0 2023-02-28 14:04:06.000000 ethos-u-vela-3.7.0/ethosu/config_files/Arm/
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     3862 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/config_files/Arm/vela.ini
-drwxr-x---   0 timhal01  (1000) timhal01  (1000)        0 2023-02-28 14:04:06.000000 ethos-u-vela-3.7.0/ethosu/mlw_codec/
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1291 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/mlw_codec/makefile
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     9389 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/mlw_codec/mlw_codecmodule.c
--rw-r-----   0 timhal01  (1000) timhal01  (1000)      958 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/mlw_codec/mlw_common.h
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    11109 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/mlw_codec/mlw_decode.c
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1089 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/mlw_codec/mlw_decode.h
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    41192 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/mlw_codec/mlw_encode.c
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1568 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/mlw_codec/mlw_encode.h
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     5347 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/mlw_codec/mlw_main.c
-drwxr-x---   0 timhal01  (1000) timhal01  (1000)        0 2023-02-28 14:04:06.000000 ethos-u-vela-3.7.0/ethosu/mlw_codec/test/
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     3234 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/mlw_codec/test/test_mlw_codec.py
-drwxr-x---   0 timhal01  (1000) timhal01  (1000)        0 2023-02-28 14:04:06.000000 ethos-u-vela-3.7.0/ethosu/vela/
--rw-r-----   0 timhal01  (1000) timhal01  (1000)      742 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/__init__.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)      759 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/__main__.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)      766 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/_version.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    18665 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/api.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    17490 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/architecture_allocator.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    35247 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/architecture_features.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    15068 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/cascade_builder.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    10191 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/compiler_driver.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     4845 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/data_type.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     6269 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/debug_database.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     5010 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/driver_actions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2725 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/errors.py
-drwxr-x---   0 timhal01  (1000) timhal01  (1000)        0 2023-02-28 14:04:06.000000 ethos-u-vela-3.7.0/ethosu/vela/ethos_u55_regs/
--rw-r-----   0 timhal01  (1000) timhal01  (1000)        0 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/ethosu/vela/ethos_u55_regs/__init__.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)   133784 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/ethos_u55_regs/ethos_u55_regs.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    10290 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/extract_npu_subgraphs.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     7626 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/fp_math.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1986 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/graph_optimiser.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    18909 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/graph_optimiser_util.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2858 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/greedy_allocation.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    11505 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/high_level_command_stream.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    10739 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/high_level_command_stream_generator.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    28373 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/high_level_command_to_npu_op.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    15685 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/hillclimb_allocation.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    15046 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/live_range.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     5564 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/lut.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     4286 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/mark_tensors.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2544 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/model_reader.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    21118 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/nn_graph.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    37417 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/npu_performance.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     6711 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/npu_serialisation.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2444 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/numeric_util.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    35609 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/operation.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     8313 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/operation_util.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    20066 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/pass_packing.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     5022 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/range_set.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     3261 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/rawdata_writer.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     3061 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/reader_util.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    47761 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/register_command_stream_generator.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    23842 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/register_command_stream_util.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     4546 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/rewrite_graph.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     3672 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/scaling.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    75808 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/scheduler.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     6802 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/shape4d.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    31099 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/softmax.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    13943 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/stats_writer.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1101 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/supported_operators_util.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    33618 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tensor.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    10851 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tensor_allocation.py
-drwxr-x---   0 timhal01  (1000) timhal01  (1000)        0 2023-02-28 14:04:06.000000 ethos-u-vela-3.7.0/ethosu/vela/test/
-drwxr-x---   0 timhal01  (1000) timhal01  (1000)        0 2023-02-28 14:04:06.000000 ethos-u-vela-3.7.0/ethosu/vela/test/extapi/
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1834 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/test/extapi/test_extapi_create_payload.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1470 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/test/extapi/test_extapi_encode_bias.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2456 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/test/extapi/test_extapi_encode_weights.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     4473 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/test/extapi/test_extapi_find_block_configs.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    19536 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/test/extapi/test_extapi_generate_commands.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1061 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/test/extapi/test_extapi_get_version.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     4335 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/test/test_architecture_allocator.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1868 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/test/test_compiler_driver.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    13053 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/test/test_fp_math.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    24795 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/test/test_graph_optimiser.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1929 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/test/test_hillclimb_allocation.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2311 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/test/test_live_range.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     8973 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/test/test_lut.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1314 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/test/test_model_reader.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     3032 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/test/test_new_performance.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1621 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/test/test_nng_mapping.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     9963 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/test/test_register_command_stream_util.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2122 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/test/test_scaling.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1775 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/test/test_tensor_allocation.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    25734 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/test/test_tflite_model_semantic.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     5209 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/test/test_tflite_reader.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    27156 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/test/test_tflite_supported_operators.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     4478 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/test/testutil.py
-drwxr-x---   0 timhal01  (1000) timhal01  (1000)        0 2023-02-28 14:04:06.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1157 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/ATan2Options.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1139 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/AbsOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)      220 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/ActivationFunctionType.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1148 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/AddNOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2148 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/AddOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1611 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/ArgMaxOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1611 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/ArgMinOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1238 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/AssignVariableOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2637 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/BatchMatMulOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1238 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/BatchToSpaceNDOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     4593 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/BidirectionalSequenceLSTMOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     3579 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/BidirectionalSequenceRNNOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1211 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/BroadcastToOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2641 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/BucketizeOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2383 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/Buffer.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     3350 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/BuiltinOperator.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     3381 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/BuiltinOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1693 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/CallOnceOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1575 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/CallOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2034 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/CastOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)      158 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/CombinerType.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     5049 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/ConcatEmbeddingsOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2219 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/ConcatenationOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     3959 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/Conv2DOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     4871 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/Conv3DOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1139 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/CosOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2044 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/CumsumOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)      146 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/CustomOptionsFormat.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2615 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/CustomQuantization.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1175 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/DensifyOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1677 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/DepthToSpaceOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     4717 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/DepthwiseConv2DOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1202 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/DequantizeOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     4301 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/DimensionMetadata.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)      153 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/DimensionType.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1679 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/DivOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1274 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/DynamicUpdateSliceOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1775 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/EmbeddingLookupSparseOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1157 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/EqualOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1139 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/ExpOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1202 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/ExpandDimsOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2914 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/FakeQuantOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1148 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/FillOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1184 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/FloorDivOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1184 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/FloorModOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     3383 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/FullyConnectedOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)      182 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/FullyConnectedOptionsWeightsFormat.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1184 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/GatherNdOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2004 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/GatherOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1605 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/GeluOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1220 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/GreaterEqualOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1175 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/GreaterOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1193 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/HardSwishOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1229 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/HashtableFindOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1247 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/HashtableImportOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2517 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/HashtableOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1229 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/HashtableSizeOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2112 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/IfOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2496 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/Int32Vector.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1715 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/L2NormOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1647 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/LSHProjectionOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)      169 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/LSHProjectionType.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)      148 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/LSTMKernelType.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     3559 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/LSTMOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1617 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/LeakyReluOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1193 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/LessEqualOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1148 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/LessOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     3231 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/LocalResponseNormalizationOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1202 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/LogSoftmaxOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1202 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/LogicalAndOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1202 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/LogicalNotOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1193 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/LogicalOrOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1202 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/MatrixDiagOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1229 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/MatrixSetDiagOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1238 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/MaximumMinimumOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1935 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/Metadata.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)      154 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/MirrorPadMode.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1599 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/MirrorPadOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     9533 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/Model.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1679 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/MulOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1139 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/NegOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1283 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/NonMaxSuppressionV4Options.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1283 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/NonMaxSuppressionV5Options.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1184 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/NotEqualOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1565 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/OneHotOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    10212 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/Operator.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     3032 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/OperatorCode.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1990 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/PackOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1139 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/PadOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1157 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/PadV2Options.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)      141 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/Padding.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     3903 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/Pool2DOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1139 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/PowOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)      166 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/QuantizationDetails.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     8544 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/QuantizationParameters.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1184 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/QuantizeOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2237 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/RNNOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1972 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/RandomOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1157 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/RangeOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1148 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/RankOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1220 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/ReadVariableOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1617 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/ReducerOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2575 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/ReshapeOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2261 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/ResizeBilinearOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2365 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/ResizeNearestNeighborOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2147 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/ReverseSequenceOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1193 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/ReverseV2Options.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1166 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/Rfft2dOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2645 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/SVDFOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1193 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/ScatterNdOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1202 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/SegmentSumOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1166 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/SelectOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1184 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/SelectV2Options.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2819 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/SequenceRNNOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1575 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/ShapeOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1148 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/SignOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     4583 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/SignatureDef.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2599 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/SkipGramOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1157 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/SliceOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1585 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/SoftmaxOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1238 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/SpaceToBatchNDOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1677 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/SpaceToDepthOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)      198 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/SparseIndexVector.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1745 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/SparseToDenseOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     5517 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/SparsityParameters.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1593 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/SplitOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1605 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/SplitVOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1166 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/SquareOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1265 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/SquaredDifferenceOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2617 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/SqueezeOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     3571 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/StridedSliceOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     6637 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/SubGraph.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2148 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/SubOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     8406 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/Tensor.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1990 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/TensorMap.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)      384 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/TensorType.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1148 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/TileOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1166 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/TopKV2Options.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2559 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/TransposeConvOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1193 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/TransposeOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2515 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/Uint16Vector.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2496 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/Uint8Vector.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     4089 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/UnidirectionalSequenceLSTMOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1611 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/UniqueOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1956 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/UnpackOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1274 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/UnsortedSegmentMaxOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1274 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/UnsortedSegmentMinOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1283 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/UnsortedSegmentProdOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1274 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/UnsortedSegmentSumOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2153 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/VarHandleOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     3367 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/VariantSubType.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1157 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/WhereOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2157 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/WhileOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1193 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/ZerosLikeOptions.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)        0 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite/__init__.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    83191 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite_graph_optimiser.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    45307 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite_mapping.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    28960 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite_model_semantic.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    14243 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite_reader.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    38489 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite_supported_operators.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    22065 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tflite_writer.py
-drwxr-x---   0 timhal01  (1000) timhal01  (1000)        0 2023-02-28 14:04:06.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa/
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1068 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa/ArithmeticRightShiftAttribute.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)      506 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa/Attribute.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)      928 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa/AxisAttribute.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1955 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa/ClampAttribute.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1376 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa/CondIfAttribute.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     3706 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa/ConvAttribute.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1280 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa/ConvQuantInfo.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)      236 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa/DType.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1264 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa/MatMulQuantInfo.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)      924 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa/MulAttribute.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1333 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa/Op.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)      932 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa/PadQuantInfo.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     3692 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa/PoolAttribute.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)      218 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa/QuantInfo.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1282 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa/ReluNAttribute.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     4499 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa/RescaleAttribute.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1657 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa/ReshapeAttribute.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     6535 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa/ResizeAttribute.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)      165 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa/ResizeMode.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2653 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa/SliceAttribute.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1652 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa/TileAttribute.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     4304 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa/TosaBasicBlock.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1964 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa/TosaGraph.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     4042 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa/TosaOperator.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     3258 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa/TosaTensor.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     4998 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa/TransposeConvAttribute.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1290 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa/UnaryQuantInfo.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1879 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa/Version.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1406 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa/WhileLoopAttribute.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)        0 2022-08-30 09:16:06.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa/__init__.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    37029 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa_graph_optimiser.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    12356 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa_mapping.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2008 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa_model_semantic.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    12661 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa_reader.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    11180 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/tosa_supported_operators.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    25452 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/vela.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)    21222 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/ethosu/vela/weight_compressor.py
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     1950 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/pyproject.toml
--rw-r-----   0 timhal01  (1000) timhal01  (1000)      220 2023-02-28 14:04:06.000000 ethos-u-vela-3.7.0/setup.cfg
--rw-r-----   0 timhal01  (1000) timhal01  (1000)     2690 2023-02-28 13:59:16.000000 ethos-u-vela-3.7.0/setup.py
+drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-05-24 15:05:53.093833 ethos-u-vela-3.8.0/
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)       94 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/.gitignore
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2119 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4268 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/API.md
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     7925 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/BUGS.md
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3245 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/CONTRIBUTIONS.md
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4115 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/DEBUG_DB.md
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    11357 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/LICENSE.txt
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    27430 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/OPTIONS.md
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    13706 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/PERFORMANCE.md
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    12381 2023-05-24 15:05:53.093833 ethos-u-vela-3.8.0/PKG-INFO
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    10280 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/README.md
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    14105 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/RELEASES.md
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     5176 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/SECURITY.md
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    19014 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/SUPPORTED_OPS.md
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3209 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/TESTING.md
+drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-05-24 15:05:53.049833 ethos-u-vela-3.8.0/ethos_u_vela.egg-info/
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    12381 2023-05-24 15:05:52.000000 ethos-u-vela-3.8.0/ethos_u_vela.egg-info/PKG-INFO
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    10736 2023-05-24 15:05:53.000000 ethos-u-vela-3.8.0/ethos_u_vela.egg-info/SOURCES.txt
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)        1 2023-05-24 15:05:52.000000 ethos-u-vela-3.8.0/ethos_u_vela.egg-info/dependency_links.txt
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)       47 2023-05-24 15:05:52.000000 ethos-u-vela-3.8.0/ethos_u_vela.egg-info/entry_points.txt
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      176 2023-05-24 15:05:52.000000 ethos-u-vela-3.8.0/ethos_u_vela.egg-info/requires.txt
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)        7 2023-05-24 15:05:52.000000 ethos-u-vela-3.8.0/ethos_u_vela.egg-info/top_level.txt
+drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-05-24 15:05:53.045832 ethos-u-vela-3.8.0/ethosu/
+drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-05-24 15:05:53.045832 ethos-u-vela-3.8.0/ethosu/config_files/
+drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-05-24 15:05:53.049833 ethos-u-vela-3.8.0/ethosu/config_files/Arm/
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3862 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/config_files/Arm/vela.ini
+drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-05-24 15:05:53.053833 ethos-u-vela-3.8.0/ethosu/mlw_codec/
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1291 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/mlw_codec/makefile
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     9389 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/mlw_codec/mlw_codecmodule.c
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      958 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/mlw_codec/mlw_common.h
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    11109 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/mlw_codec/mlw_decode.c
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1089 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/mlw_codec/mlw_decode.h
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    41192 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/mlw_codec/mlw_encode.c
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1568 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/mlw_codec/mlw_encode.h
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     5347 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/mlw_codec/mlw_main.c
+drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-05-24 15:05:53.053833 ethos-u-vela-3.8.0/ethosu/mlw_codec/test/
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3234 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/mlw_codec/test/test_mlw_codec.py
+drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-05-24 15:05:53.061833 ethos-u-vela-3.8.0/ethosu/vela/
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      742 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/__init__.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      759 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/__main__.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      766 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/_version.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    18665 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/api.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    17490 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/architecture_allocator.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    35247 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/architecture_features.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    15473 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/cascade_builder.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    11098 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/compiler_driver.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4845 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/data_type.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     6269 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/debug_database.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     5010 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/driver_actions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2725 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/errors.py
+drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-05-24 15:05:53.061833 ethos-u-vela-3.8.0/ethosu/vela/ethos_u55_regs/
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)        0 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/ethos_u55_regs/__init__.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)   133784 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/ethos_u55_regs/ethos_u55_regs.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    10290 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/extract_npu_subgraphs.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     7626 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/fp_math.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1986 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/graph_optimiser.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    13005 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/graph_optimiser_util.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2858 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/greedy_allocation.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    11920 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/high_level_command_stream.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    11652 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/high_level_command_stream_generator.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    29622 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/high_level_command_to_npu_op.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    15685 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/hillclimb_allocation.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    15911 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/live_range.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    17919 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/lstm.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    10255 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/lut.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4607 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/mark_tensors.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2544 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/model_reader.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    21118 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/nn_graph.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    38217 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/npu_performance.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     6711 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/npu_serialisation.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2444 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/numeric_util.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    37513 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/operation.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    11505 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/operation_util.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    20676 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/pass_packing.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     5022 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/range_set.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3261 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/rawdata_writer.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3098 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/reader_util.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    47761 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/register_command_stream_generator.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    23842 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/register_command_stream_util.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4546 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/rewrite_graph.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3672 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/scaling.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    76797 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/scheduler.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     6802 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/shape4d.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    31094 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/softmax.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    13943 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/stats_writer.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1101 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/supported_operators_util.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    33552 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tensor.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    10993 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tensor_allocation.py
+drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-05-24 15:05:53.065833 ethos-u-vela-3.8.0/ethosu/vela/test/
+drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-05-24 15:05:53.065833 ethos-u-vela-3.8.0/ethosu/vela/test/extapi/
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1834 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/extapi/test_extapi_create_payload.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1470 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/extapi/test_extapi_encode_bias.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2456 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/extapi/test_extapi_encode_weights.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4473 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/extapi/test_extapi_find_block_configs.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    19536 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/extapi/test_extapi_generate_commands.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1061 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/extapi/test_extapi_get_version.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4335 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/test_architecture_allocator.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2826 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/test_build.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1868 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/test_compiler_driver.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    13053 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/test_fp_math.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    24795 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/test_graph_optimiser.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1929 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/test_hillclimb_allocation.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2311 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/test_live_range.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     8952 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/test_lut.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1314 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/test_model_reader.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3032 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/test_new_performance.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1621 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/test_nng_mapping.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     9963 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/test_register_command_stream_util.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2122 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/test_scaling.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1775 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/test_tensor_allocation.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    27177 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/test_tflite_model_semantic.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     5272 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/test_tflite_reader.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    28590 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/test_tflite_supported_operators.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     6645 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/test/testutil.py
+drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-05-24 15:05:53.089833 ethos-u-vela-3.8.0/ethosu/vela/tflite/
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1157 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ATan2Options.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1139 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/AbsOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      220 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ActivationFunctionType.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1148 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/AddNOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2148 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/AddOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1611 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ArgMaxOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1611 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ArgMinOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1238 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/AssignVariableOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2637 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/BatchMatMulOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1238 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/BatchToSpaceNDOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4593 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/BidirectionalSequenceLSTMOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3579 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/BidirectionalSequenceRNNOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1211 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/BroadcastToOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2641 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/BucketizeOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2383 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/Buffer.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3350 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/BuiltinOperator.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3381 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/BuiltinOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1693 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/CallOnceOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1575 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/CallOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2034 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/CastOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      158 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/CombinerType.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     5049 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ConcatEmbeddingsOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2219 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ConcatenationOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3959 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/Conv2DOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4871 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/Conv3DOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1139 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/CosOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2044 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/CumsumOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      146 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/CustomOptionsFormat.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2615 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/CustomQuantization.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1175 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/DensifyOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1677 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/DepthToSpaceOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4717 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/DepthwiseConv2DOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1202 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/DequantizeOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4301 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/DimensionMetadata.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      153 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/DimensionType.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1679 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/DivOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1274 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/DynamicUpdateSliceOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1775 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/EmbeddingLookupSparseOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1157 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/EqualOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1139 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ExpOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1202 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ExpandDimsOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2914 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/FakeQuantOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1148 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/FillOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1184 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/FloorDivOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1184 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/FloorModOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3383 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/FullyConnectedOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      182 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/FullyConnectedOptionsWeightsFormat.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1184 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/GatherNdOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2004 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/GatherOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1605 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/GeluOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1220 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/GreaterEqualOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1175 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/GreaterOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1193 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/HardSwishOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1229 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/HashtableFindOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1247 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/HashtableImportOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2517 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/HashtableOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1229 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/HashtableSizeOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2112 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/IfOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2496 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/Int32Vector.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1715 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/L2NormOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1647 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/LSHProjectionOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      169 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/LSHProjectionType.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      148 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/LSTMKernelType.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3559 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/LSTMOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1617 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/LeakyReluOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1193 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/LessEqualOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1148 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/LessOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3231 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/LocalResponseNormalizationOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1202 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/LogSoftmaxOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1202 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/LogicalAndOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1202 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/LogicalNotOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1193 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/LogicalOrOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1202 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/MatrixDiagOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1229 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/MatrixSetDiagOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1238 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/MaximumMinimumOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1935 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/Metadata.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      154 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/MirrorPadMode.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1599 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/MirrorPadOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     9533 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/Model.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1679 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/MulOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1139 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/NegOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1283 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/NonMaxSuppressionV4Options.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1283 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/NonMaxSuppressionV5Options.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1184 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/NotEqualOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1565 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/OneHotOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    10212 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/Operator.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3032 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/OperatorCode.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1990 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/PackOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1139 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/PadOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1157 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/PadV2Options.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      141 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/Padding.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3903 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/Pool2DOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1139 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/PowOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      166 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/QuantizationDetails.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     8544 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/QuantizationParameters.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1184 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/QuantizeOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2237 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/RNNOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1972 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/RandomOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1157 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/RangeOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1148 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/RankOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1220 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ReadVariableOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1617 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ReducerOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2575 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ReshapeOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2261 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ResizeBilinearOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2365 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ResizeNearestNeighborOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2147 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ReverseSequenceOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1193 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ReverseV2Options.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1166 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/Rfft2dOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2645 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SVDFOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1193 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ScatterNdOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1202 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SegmentSumOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1166 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SelectOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1184 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SelectV2Options.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2819 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SequenceRNNOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1575 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ShapeOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1148 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SignOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4583 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SignatureDef.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2599 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SkipGramOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1157 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SliceOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1585 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SoftmaxOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1238 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SpaceToBatchNDOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1677 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SpaceToDepthOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      198 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SparseIndexVector.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1745 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SparseToDenseOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     5517 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SparsityParameters.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1593 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SplitOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1605 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SplitVOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1166 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SquareOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1265 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SquaredDifferenceOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2617 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SqueezeOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3571 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/StridedSliceOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     6637 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SubGraph.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2148 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/SubOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     8406 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/Tensor.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1990 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/TensorMap.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      398 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/TensorType.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1148 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/TileOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1166 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/TopKV2Options.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3130 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/TransposeConvOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1193 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/TransposeOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2515 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/Uint16Vector.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2496 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/Uint8Vector.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4089 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/UnidirectionalSequenceLSTMOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1611 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/UniqueOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1956 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/UnpackOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1274 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/UnsortedSegmentMaxOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1274 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/UnsortedSegmentMinOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1283 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/UnsortedSegmentProdOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1274 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/UnsortedSegmentSumOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2153 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/VarHandleOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3367 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/VariantSubType.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1157 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/WhereOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2157 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/WhileOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1193 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/ZerosLikeOptions.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)        0 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite/__init__.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)   100599 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite_graph_optimiser.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    46097 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite_mapping.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    32755 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite_model_semantic.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    16397 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite_reader.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    39946 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite_supported_operators.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    22790 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tflite_writer.py
+drwxr-xr-x   0 ricbol01 (30336) devsysle   (431)        0 2023-05-24 15:05:53.093833 ethos-u-vela-3.8.0/ethosu/vela/tosa/
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1068 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/ArithmeticRightShiftAttribute.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      506 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/Attribute.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      928 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/AxisAttribute.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1955 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/ClampAttribute.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1376 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/CondIfAttribute.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3706 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/ConvAttribute.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1280 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/ConvQuantInfo.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      236 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/DType.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1264 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/MatMulQuantInfo.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      924 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/MulAttribute.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1333 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/Op.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      932 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/PadQuantInfo.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3692 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/PoolAttribute.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      218 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/QuantInfo.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1282 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/ReluNAttribute.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4499 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/RescaleAttribute.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1657 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/ReshapeAttribute.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     6535 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/ResizeAttribute.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      165 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/ResizeMode.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2653 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/SliceAttribute.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1652 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/TileAttribute.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4304 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/TosaBasicBlock.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1964 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/TosaGraph.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4042 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/TosaOperator.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3258 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/TosaTensor.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     4998 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/TransposeConvAttribute.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1290 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/UnaryQuantInfo.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1879 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/Version.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     1406 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/WhileLoopAttribute.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)        0 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa/__init__.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    37007 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa_graph_optimiser.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    12356 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa_mapping.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2008 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa_model_semantic.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    12661 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa_reader.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    11180 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/tosa_supported_operators.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     3481 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/utils.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    26621 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/vela.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)    20790 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/ethosu/vela/weight_compressor.py
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2095 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/pyproject.toml
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)      220 2023-05-24 15:05:53.093833 ethos-u-vela-3.8.0/setup.cfg
+-rw-r--r--   0 ricbol01 (30336) devsysle   (431)     2735 2023-05-24 14:51:33.000000 ethos-u-vela-3.8.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ethos-u-vela-3.7.0/API.md` & `ethos-u-vela-3.8.0/API.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+<!--
+SPDX-FileCopyrightText: Copyright 2020, 2023 Arm Limited and/or its affiliates <open-source-office@arm.com>
+
+SPDX-License-Identifier: Apache-2.0
+
+Licensed under the Apache License, Version 2.0 (the License); you may
+not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an AS IS BASIS, WITHOUT
+WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+-->
 # Vela External APIs
 
 Vela provides a low-level external API to enable Ethos-U code generation from
 other tools.
 
 The external APIs facilitate other tools that require backend compiler
 functionality. From herein this functionality is referred to as "the compiler".
```

### Comparing `ethos-u-vela-3.7.0/BUGS.md` & `ethos-u-vela-3.8.0/BUGS.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+<!--
+SPDX-FileCopyrightText: Copyright 2021, 2023 Arm Limited and/or its affiliates <open-source-office@arm.com>
+
+SPDX-License-Identifier: Apache-2.0
+
+Licensed under the Apache License, Version 2.0 (the License); you may
+not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an AS IS BASIS, WITHOUT
+WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+-->
 # Vela Community Bug Reporting
 
 If the Vela community encounters a bug, then we highly encourage the community
 to report it. When issuing a report, use the
 [Maniphest bug tracker](https://developer.mlplatform.org/maniphest/)
 that is part of Phabricator on ML Platform. This site enables any Vela user to
 discuss and share any Vela related issue with the community.
```

### Comparing `ethos-u-vela-3.7.0/CONTRIBUTIONS.md` & `ethos-u-vela-3.8.0/CONTRIBUTIONS.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+<!--
+SPDX-FileCopyrightText: Copyright 2020-2023 Arm Limited and/or its affiliates <open-source-office@arm.com>
+
+SPDX-License-Identifier: Apache-2.0
+
+Licensed under the Apache License, Version 2.0 (the License); you may
+not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an AS IS BASIS, WITHOUT
+WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+-->
 # Vela Contributions
 
 Contributions to Vela are very much welcomed!
 
 ## Coding Standard
 
 Vela is written using Python 3.7 language constructs in order to aid
```

### Comparing `ethos-u-vela-3.7.0/DEBUG_DB.md` & `ethos-u-vela-3.8.0/DEBUG_DB.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+<!--
+SPDX-FileCopyrightText: Copyright 2021, 2023 Arm Limited and/or its affiliates <open-source-office@arm.com>
+
+SPDX-License-Identifier: Apache-2.0
+
+Licensed under the Apache License, Version 2.0 (the License); you may
+not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an AS IS BASIS, WITHOUT
+WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+-->
 # Vela Debug Database
 
 The purpose of the debug database is to track operator transformations during
 the optimisation process of Vela.  This is later correlated with the trace
 output of the model, externally, to determine the runtime of the original layer
 operators.  Standalone, the debug database can be used in order to give a brief
 overview of how the operators in the network change throughout the optimisation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-# Vela Debug Database The purpose of the debug database is to track operator
+ # Vela Debug Database The purpose of the debug database is to track operator
 transformations during the optimisation process of Vela. This is later
 correlated with the trace output of the model, externally, to determine the
 runtime of the original layer operators. Standalone, the debug database can be
 used in order to give a brief overview of how the operators in the network
 change throughout the optimisation process. This document gives an overview of
 the structure of the database and its outputs, to help parsing of the generated
 data in a debug procedure. ## Contents While processing, Vela maintains
```

### Comparing `ethos-u-vela-3.7.0/LICENSE.txt` & `ethos-u-vela-3.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/OPTIONS.md` & `ethos-u-vela-3.8.0/OPTIONS.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+<!--
+SPDX-FileCopyrightText: Copyright 2020-2023 Arm Limited and/or its affiliates <open-source-office@arm.com>
+
+SPDX-License-Identifier: Apache-2.0
+
+Licensed under the Apache License, Version 2.0 (the License); you may
+not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an AS IS BASIS, WITHOUT
+WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+-->
 # Vela Options
 
 This file contains a more verbose and detailed description of the Vela
 Compiler's CLI options than the built-in help strings.  It also defines and
 describes Vela's configuration file format.
 
 ## Command Line Interface
@@ -315,31 +332,57 @@
 
 ```bash
 vela network.tflite --verbose-config
 ```
 
 ### Verbose Graph
 
-Verbose graph rewriter.  
+Displays two lists of operators. The first lists all of the operators that exist
+in Vela's internal representation (Graph IR) of the Neural Network Graph (NNG)
+before the graph optimisation process has run.  The second lists all of the
+operators after that process.  The lists do not show the connectivity
+information of the NNG and are unordered, therefore the execution order may
+differ.  Each line in the list is of the format:  
+`<num> <op_type> <op_name>`, where;  
+num = an increasing operator count  
+op_type = the Graph IR Operator Type  
+op_name = the Graph IR Operator Name (this may have been derived from the
+corresponding TFLite operator name)  
 
 ```bash
 vela network.tflite --verbose-graph
 ```
 
 ### Verbose Quantization
 
-Verbose quantization.  
+Displays quantization information of all *weight*, *bias*, *input* and *output*
+tensors for each operator in the Neural Network Graph (NNG).  The quantization
+approximates floating point values as:
+`approx_float_value = (integer_value - zero_point) * scale`
+The information of each tensor is displayed in the format:
+`<idx> <data_type> <min> <max> <scale> <zero_point> <name>`, where;  
+idx = the tensor index on each operator  
+min = the minimum floating point value before quantization  
+max = the maximum floating point value before quantization  
+scale = the quantization scaling, zero_point = the quantization zero point  
+name = the name of the tensor  
 
 ```bash
 vela network.tflite --verbose-quantization
 ```
 
 ### Verbose Packing
 
-Verbose pass packing.  
+Displays a list of passes where a pass represents one or more Graph IR operators
+that are run together as one hardware operation e.g. a pass could be a
+convolution operator fused with a hardswish activation.  Each line of the list
+has the format:  
+`<id> <pass>`, where;  
+id = an increasing pass count  
+pass = name of the pass (usually derived from the first operator in the pass)  
 
 ```bash
 vela network.tflite --verbose-packing
 ```
 
 ### Verbose Performance
 
@@ -349,76 +392,131 @@
 
 ```bash
 vela network.tflite --verbose-performance
 ```
 
 ### Verbose Tensor Purpose
 
-Verbose tensor purpose.  
+Displays a list of all operators and the tensors that are connected to them.
+Additional information is shown about the tensors. The format is:
+`<num> <op_type> <op_name>`, where;  
+`  <direction> <idx> <purpose> <mem_area> <mem_type> <tens>`, where;  
+num = an increasing operator count  
+op_type = the Graph IR Operator Type  
+op_name = the Graph IR Operator Name (this may have been derived from the
+corresponding TFLite operator name)  
+direction = either *Input* or *Output* and indicates the connection direction of
+the tensor with respect 
+idx = the index position where on each operator  
+purpose = purpose of the tensor (weight, bias, feature map, etc.)  
+mem_area = assigned memory area (for example SRAM or Flash)  
+mem_type = memory type (i.e. Scratch or Permanent NPU)  
+tens = string representation of the tensor containing its name, shape and data
+type  
 
 ```bash
 vela network.tflite --verbose-tensor-purpose
 ```
 
-### Verbose Tensor Format
-
-Verbose tensor format.  
-
-```bash
-vela network.tflite --verbose-tensor-format
-```
-
 ### Verbose Schedule
 
-Verbose schedule.  
+Display all schedule operations which contain information about the operator
+type, block config, stripe sizes, size of encoded weights, size of weight
+buffers, depth slices, cascade assignment and SRAM usage. The purpose of the
+scheduler is to come up with an execution plan for the network. It will make
+decisions on how to split an operator execution into stripes, group operators
+together in cascades to either reduce SRAM footprint or, in a multi-level
+memory system, better utilize the SRAM. The scheduler will also decide in what
+memory to put tensors as well as how to buffer data from a slower memory like
+Flash/DRAM to SRAM.
+
+Feature maps can be split up into horizontal subsections called stripes that
+allow us to apply operators independently to smaller sections of feature maps.
+The output stripes that are produced can fit into a smaller buffer than the
+output of a full feature map would, which combined with cascading can reduce
+memory usage.
+
+A cascade is a group of operators that will be computed interleaved in stripes.
+Instead of storing the full output of an operator applied on a whole feature
+map, we calculate the smallest possible buffer that allows storing intermediate
+results of enough output stripes of one operator to allow the consecutive
+operator to calculate one output stripe. Then, the consumed parts of the buffer
+that is no longer needed by the consecutive operator in the cascade can be
+overwritten by a new output stripe of the first operator, allowing us to reuse
+and reduce the memory usage.  
 
 ```bash
 vela network.tflite --verbose-schedule
 ```
 
 ### Verbose Allocation
 
-Verbose tensor allocation.  
+This option displays tensor allocation information in separate tables for each
+type of memory area. Each table contains information about each tensor's start
+and end time, address, size and purpose as well as the memory usage during the
+each tensors live range. The start- and end time denotes the time steps during
+when the tensor needs to be allocated in the memory. After the end time, the
+addresses are allowed to be overwritten by other tensors. The reported memory
+usage is the peak usage at any time step of the tensors live range, which means
+that the maximum memory usage value of all tensors will be the minimum required
+size to fit the proposed allocation.  
 
 ```bash
 vela network.tflite --verbose-allocation
 ```
 
 ### Verbose High Level Command Stream
 
-Verbose high level command stream.  
+Display a high level command stream with one command per DMA or NPU stripe. The
+commands contain information about block configuration as well as IFM-, OFM-
+and weight boxes.  
 
 ```bash
 vela network.tflite --verbose-high-level-command-stream
 ```
 
 ### Verbose Register Command Stream
 
-Verbose register command stream.  
+Display all NPU operations and a register level (low level) command stream with
+all register settings for the network execution on the NPU.  
 
 ```bash
 vela network.tflite --verbose-register-command-stream
 ```
 
 ### Verbose Operators
 
-Verbose operator list.  
+Display a list of all operators in the neural network graph along with their
+attributes before any optimization is made by Vela.  
 
 ```bash
 vela network.tflite --verbose-operators
 ```
 
 ### Verbose Weights
 
-Verbose weights information.  
+Displays the size of the *Original* and *Ethos-U NPU Encoded* weights as part of
+the final summary information.  The *original* weights size refers to the size
+of the weights as read from the input `.tflite` file.  The *NPU Encoded* weights
+size refers to the total size of all of the weight tensors after they have been
+reordered, padded and encoded for the operators that run on the Ethos-U.  
 
 ```bash
 vela network.tflite --verbose-weights
 ```
 
+### Verbose Progress
+
+This option displays progress information of the most time consuming parts of
+the compiler driver and scheduler.  
+
+```bash
+vela network.tflite --verbose-progress
+```
+
 ## Configuration File
 
 This is used to describe various properties of the Ethos-U embedded system.  The
 configuration file is selected using the `--config` CLI option along with a file
 that describes the properties.  The format of the file is a Python ConfigParser
 `.ini` file format consists of sections used to identify a configuration, and
 key/value pair options used to specify the properties.  All sections and
```

### Comparing `ethos-u-vela-3.7.0/PERFORMANCE.md` & `ethos-u-vela-3.8.0/PERFORMANCE.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+<!--
+SPDX-FileCopyrightText: Copyright 2021-2023 Arm Limited and/or its affiliates <open-source-office@arm.com>
+
+SPDX-License-Identifier: Apache-2.0
+
+Licensed under the Apache License, Version 2.0 (the License); you may
+not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an AS IS BASIS, WITHOUT
+WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+-->
 # Vela Performance Estimation Summary
 
 This is a description of the performance estimation summary that Vela prints
 after each compilation.  This summary is also printed to a csv in the output
 directory.
 
 The following is an example of the output.
```

### Comparing `ethos-u-vela-3.7.0/PKG-INFO` & `ethos-u-vela-3.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,47 @@
 Metadata-Version: 2.1
 Name: ethos-u-vela
-Version: 3.7.0
+Version: 3.8.0
 Summary: Neural network model compiler for Arm Ethos-U NPUs
 Author-email: Arm Ltd <mlg-vela@arm.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://git.mlplatform.org/ml/ethos-u/ethos-u-vela.git/
 Keywords: ethos-u,vela compiler,tflite,npu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Compilers
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE.txt
 
+<!--
+SPDX-FileCopyrightText: Copyright 2020-2023 Arm Limited and/or its affiliates <open-source-office@arm.com>
+
+SPDX-License-Identifier: Apache-2.0
+
+Licensed under the Apache License, Version 2.0 (the License); you may
+not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an AS IS BASIS, WITHOUT
+WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+-->
 # Vela
 
 This tool is used to compile a
 [TensorFlow Lite for Microcontrollers](https://www.tensorflow.org/lite/microcontrollers)
 neural network model into an optimised version that can run on an embedded
 system containing an
 [Arm Ethos-U NPU](https://www.arm.com/products/silicon-ip-cpu).
@@ -46,16 +64,16 @@
 compiled model.
 
 The tool has limited functionality for compiling a
 [TOSA](https://git.mlplatform.org/tosa/specification.git/) neural network
 (EXPERIMENTAL).
 
 ## TensorFlow Support
-
-* Vela 3.6.0 to current supports TensorFlow 2.10
+* Vela 3.8.0 to current supports TensorFlow 2.11
+* Vela 3.6.0 to 3.7.0 supports TensorFlow 2.10
 * Vela 3.5.0 supports TensorFlow 2.9
 * Vela 3.4.0 supports TensorFlow 2.8
 * Vela 3.3.0 supports TensorFlow 2.7
 * Vela 3.1.0 to 3.2.0 supports TensorFlow 2.5
 * Vela 2.1.0 to 3.0.0 supports TensorFlow 2.4
 * Vela 2.0.0 to 2.0.1 supports TensorFlow 2.3
 * Vela 0.1.0 to 1.2.0 supports TensorFlow 2.1
@@ -64,17 +82,17 @@
 
 Vela runs on Linux and Microsoft Windows 10 operating systems.
 
 ## Prerequisites
 
 The following should be installed prior to the installation of Vela:
 
-* Python 3.7 or compatible
+* Python 3.9 or compatible
    - Development version containing the Python/C API header files
-   - e.g. `apt install python3.7-dev` or `yum install python37-devel`
+   - e.g. `apt install python3.9-dev` or `yum install python39-devel`
 * Pip3
 * A C99 capable compiler and associated toolchain
     - For Linux operating systems, a GNU toolchain is recommended.
     - For Microsoft Windows 10, Microsoft Visual C++ 14.2 Build Tools is recommended.
       See <https://wiki.python.org/moin/WindowsCompilers>
 
 ## Installation
@@ -118,25 +136,25 @@
 This is done by adding the `-e` option to the install command like so:
 
 ```bash
 pip3 install -e .
 ```
 
 If you plan to contribute to the Vela project (highly encouraged!) then it is
-recommended to install Vela along with the pre-commit tools (see
-[Vela Testing](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.7.0/TESTING.md) for more details).
+recommended to install Vela with the development dependencies (see
+[Vela Testing](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/TESTING.md) for more details).
 
 ## Running
 
 Vela is run with an input `.tflite` or `.tosa` (EXPERIMENTAL) file passed on the
 command line. This file contains the neural network to be compiled. The tool then
 outputs an optimised `.tflite` file with a `_vela` suffix in the file name, along
 with performance estimate (EXPERIMENTAL) CSV files, all to the output directory.
 It also prints a performance estimation summary back to the console, see
-[Vela Performance Estimation Summary](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.7.0/PERFORMANCE.md).
+[Vela Performance Estimation Summary](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/PERFORMANCE.md).
 
 Example usage:
 
 1) Compile the network `my_model.tflite`.  The optimised version will be output
 to `./output/my_network_vela.tflite`.
 
 ```bash
@@ -223,15 +241,15 @@
 the mlw_codec and the current version of NumPy.
 
 **Example scenario:**
 
 In the ethos-u-vela source directory, run:
 
 ```bash
-virtualenv -p 3.8 venv
+virtualenv -p 3.9 venv
 . venv/bin/activate
 pip install ethos-u-vela
 ```
 
 Next, install a different NumPy version (e.g. 1.21.3)
 
 ```bash
@@ -269,66 +287,66 @@
    in mlw_codec during the build process.
    ```
    pip install ethos-u-vela --no-build-isolation --no-cache-dir
    ```
 
 ## APIs
 
-Please see [Vela External APIs](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.7.0/API.md).
+Please see [Vela External APIs](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/API.md).
 
 ## Bug Reporting
 
-Please see [Vela Community Bug Reporting](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.7.0/BUGS.md) for a description of how to
+Please see [Vela Community Bug Reporting](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/BUGS.md) for a description of how to
 report bugs.
 
 ## Contributions
 
-Please see [Vela Contributions](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.7.0/CONTRIBUTIONS.md).
+Please see [Vela Contributions](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/CONTRIBUTIONS.md).
 
 ## Debug Database
 
-Please see [Vela Debug Database](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.7.0/DEBUG_DB.md).
+Please see [Vela Debug Database](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/DEBUG_DB.md).
 
 ## Inclusive language commitment
 
 This product conforms to Arm’s inclusive language policy and, to the best of
 our knowledge, does not contain any non-inclusive language. If you find
 something that concerns you, email terms@arm.com.
 
 ## Options
 
-Please see [Vela CLI Options](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.7.0/OPTIONS.md).  This includes a description of the
+Please see [Vela CLI Options](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/OPTIONS.md).  This includes a description of the
 system configuration file format.
 
 ## Performance
 
-Please see [Vela Performance Estimation Summary](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.7.0/PERFORMANCE.md).
+Please see [Vela Performance Estimation Summary](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/PERFORMANCE.md).
 
 ## Releases
 
-Please see [Vela Releases](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.7.0/RELEASES.md).
+Please see [Vela Releases](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/RELEASES.md).
 
 ## Resources
 
 Additional useful information:
 
 * [Arm Products: Ethos-U55 NPU](https://www.arm.com/products/silicon-ip-cpu/ethos/ethos-u55)
 * [Arm Products: Ethos-U65 NPU](https://www.arm.com/products/silicon-ip-cpu/ethos/ethos-u65)
 * [Arm Developer: Ethos-U55 NPU](https://developer.arm.com/ip-products/processors/machine-learning/arm-ethos-u/ethos-u55)
 * [Arm Developer: Ethos-U65 NPU](https://developer.arm.com/ip-products/processors/machine-learning/arm-ethos-u/ethos-u65)
 
 ## Security
 
-Please see [Vela Security](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.7.0/SECURITY.md).
+Please see [Vela Security](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/SECURITY.md).
 
 ## Supported Operators
 
-Please see [Vela Supported Operators](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.7.0/SUPPORTED_OPS.md) for the list of
+Please see [Vela Supported Operators](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/SUPPORTED_OPS.md) for the list of
 operators supported in this release.
 
 ## Testing
 
-Please see [Vela Testing](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.7.0/TESTING.md).
+Please see [Vela Testing](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/TESTING.md).
 
 ## License
 
-Vela is licensed under [Apache License 2.0](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.7.0/LICENSE.txt).
+Vela is licensed under [Apache License 2.0](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/LICENSE.txt).
```

### Comparing `ethos-u-vela-3.7.0/README.md` & `ethos-u-vela-3.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+<!--
+SPDX-FileCopyrightText: Copyright 2020-2023 Arm Limited and/or its affiliates <open-source-office@arm.com>
+
+SPDX-License-Identifier: Apache-2.0
+
+Licensed under the Apache License, Version 2.0 (the License); you may
+not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an AS IS BASIS, WITHOUT
+WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+-->
 # Vela
 
 This tool is used to compile a
 [TensorFlow Lite for Microcontrollers](https://www.tensorflow.org/lite/microcontrollers)
 neural network model into an optimised version that can run on an embedded
 system containing an
 [Arm Ethos-U NPU](https://www.arm.com/products/silicon-ip-cpu).
@@ -24,16 +41,16 @@
 compiled model.
 
 The tool has limited functionality for compiling a
 [TOSA](https://git.mlplatform.org/tosa/specification.git/) neural network
 (EXPERIMENTAL).
 
 ## TensorFlow Support
-
-* Vela 3.6.0 to current supports TensorFlow 2.10
+* Vela 3.8.0 to current supports TensorFlow 2.11
+* Vela 3.6.0 to 3.7.0 supports TensorFlow 2.10
 * Vela 3.5.0 supports TensorFlow 2.9
 * Vela 3.4.0 supports TensorFlow 2.8
 * Vela 3.3.0 supports TensorFlow 2.7
 * Vela 3.1.0 to 3.2.0 supports TensorFlow 2.5
 * Vela 2.1.0 to 3.0.0 supports TensorFlow 2.4
 * Vela 2.0.0 to 2.0.1 supports TensorFlow 2.3
 * Vela 0.1.0 to 1.2.0 supports TensorFlow 2.1
@@ -42,17 +59,17 @@
 
 Vela runs on Linux and Microsoft Windows 10 operating systems.
 
 ## Prerequisites
 
 The following should be installed prior to the installation of Vela:
 
-* Python 3.7 or compatible
+* Python 3.9 or compatible
    - Development version containing the Python/C API header files
-   - e.g. `apt install python3.7-dev` or `yum install python37-devel`
+   - e.g. `apt install python3.9-dev` or `yum install python39-devel`
 * Pip3
 * A C99 capable compiler and associated toolchain
     - For Linux operating systems, a GNU toolchain is recommended.
     - For Microsoft Windows 10, Microsoft Visual C++ 14.2 Build Tools is recommended.
       See <https://wiki.python.org/moin/WindowsCompilers>
 
 ## Installation
@@ -96,15 +113,15 @@
 This is done by adding the `-e` option to the install command like so:
 
 ```bash
 pip3 install -e .
 ```
 
 If you plan to contribute to the Vela project (highly encouraged!) then it is
-recommended to install Vela along with the pre-commit tools (see
+recommended to install Vela with the development dependencies (see
 [Vela Testing](TESTING.md) for more details).
 
 ## Running
 
 Vela is run with an input `.tflite` or `.tosa` (EXPERIMENTAL) file passed on the
 command line. This file contains the neural network to be compiled. The tool then
 outputs an optimised `.tflite` file with a `_vela` suffix in the file name, along
@@ -201,15 +218,15 @@
 the mlw_codec and the current version of NumPy.
 
 **Example scenario:**
 
 In the ethos-u-vela source directory, run:
 
 ```bash
-virtualenv -p 3.8 venv
+virtualenv -p 3.9 venv
 . venv/bin/activate
 pip install ethos-u-vela
 ```
 
 Next, install a different NumPy version (e.g. 1.21.3)
 
 ```bash
```

### Comparing `ethos-u-vela-3.7.0/RELEASES.md` & `ethos-u-vela-3.8.0/RELEASES.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,58 @@
+<!--
+SPDX-FileCopyrightText: Copyright 2020-2023 Arm Limited and/or its affiliates <open-source-office@arm.com>
+
+SPDX-License-Identifier: Apache-2.0
+
+Licensed under the Apache License, Version 2.0 (the License); you may
+not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an AS IS BASIS, WITHOUT
+WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+-->
 # Vela Releases
 
 These are the release notes for all Vela releases.  They document all of the
 main feature changes, interface changes and reported defects that have been
 fixed.  The version numbering adheres to the
 [semantic versioning](https://semver.org/) scheme.
 
+## Release 3.8.0 - 17/05/2023
+
+**Main feature changes:**
+
+* New operator support: ARG_MAX, UNIDIRECTIONAL_SEQUENCE_LSTM, EXP
+* Improved CONV_2D striding support
+* Upgrade TensorFlow Lite support to version 2.11
+* Changed MEAN operator implementation to match changes in TensorFlow Lite reference kernels
+* Fixed int8 and int16 fusing of PAD and AVERAGE_POOL_2D
+* Fixed issues with pass-through support for:
+  * Resource variables
+  * Fused activation attribute and missing attributes
+* Improved documentation of verbose CLI options
+
+**Interface changes:**
+
+* Addition of CLI options:
+  * `--verbose-progress`
+
+**Reported defect fixes:**
+
+* Compilation progress feedback (MLCE-1009)
+* Reduced compilation time for large networks (MLCE-1009)
+* Fixed handling of invalid RESHAPE operators (MLCE-997)
+* Fixed crash when passing-through semantically incorrect operators with missing attributes (MLCE-1027)
+
+
 ## Release 3.7.0 - 16/02/2023
 
 **Main feature changes:**
 
 * Added support for Tensor is_variable attribute
   * Requires TensorFlow Lite for Microcontrollers PR#1676 see
     <https://github.com/tensorflow/tflite-micro/pull/1676>
```

### Comparing `ethos-u-vela-3.7.0/SECURITY.md` & `ethos-u-vela-3.8.0/SECURITY.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+<!--
+SPDX-FileCopyrightText: Copyright 2020-2021, 2023 Arm Limited and/or its affiliates <open-source-office@arm.com>
+
+SPDX-License-Identifier: Apache-2.0
+
+Licensed under the Apache License, Version 2.0 (the License); you may
+not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an AS IS BASIS, WITHOUT
+WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+-->
 # Vela Security
 
 If you believe you have identified a security related issue or vulnerability,
 then we encourage you to responsibly disclose it to us as soon as possible.
 
 ## Reporting vulnerabilities
```

### Comparing `ethos-u-vela-3.7.0/SUPPORTED_OPS.md` & `ethos-u-vela-3.8.0/SUPPORTED_OPS.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,29 @@
+<!--
+SPDX-FileCopyrightText: Copyright 2020-2023 Arm Limited and/or its affiliates <open-source-office@arm.com>
+
+SPDX-License-Identifier: Apache-2.0
+
+Licensed under the Apache License, Version 2.0 (the License); you may
+not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an AS IS BASIS, WITHOUT
+WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+-->
+
 # Supported Ops
 
 This file was automatically generated by Vela using the `--supported-ops-report` parameter.  
-Vela version: `3.7.0`
+Vela version: `3.8.0`
 
 This file complies with
 [**Gitiles Markdown syntax**](https://github.com/google/gitiles/blob/master/Documentation/markdown.md)
 
 Summary table of constraints for:
 - [TFLite](#tflite-summary-table)
 
@@ -16,18 +34,20 @@
 For any other TFLite operator not listed, will be left untouched and scheduled on the CPU.  
 Please check the supported operator list for your chosen runtime for further information.
 
 | Operator | TFLite Constraints |
 | --- | --- |
 | ABS | [Generic](#tflite-generic-constraints), [Specific](#tflite-abs-constraints) |
 | ADD | [Generic](#tflite-generic-constraints), [Specific](#tflite-add-constraints) |
+| ARG_MAX | [Generic](#tflite-generic-constraints), [Specific](#tflite-arg_max-constraints) |
 | AVERAGE_POOL_2D | [Generic](#tflite-generic-constraints), [Specific](#tflite-average_pool_2d-constraints) |
 | CONCATENATION | [Generic](#tflite-generic-constraints), [Specific](#tflite-concatenation-constraints) |
 | CONV_2D | [Generic](#tflite-generic-constraints), [Specific](#tflite-conv_2d-constraints) |
 | DEPTHWISE_CONV_2D | [Generic](#tflite-generic-constraints), [Specific](#tflite-depthwise_conv_2d-constraints) |
+| EXP | [Generic](#tflite-generic-constraints), [Specific](#tflite-exp-constraints) |
 | EXPAND_DIMS | [Generic](#tflite-generic-constraints), [Specific](#tflite-expand_dims-constraints) |
 | FULLY_CONNECTED | [Generic](#tflite-generic-constraints), [Specific](#tflite-fully_connected-constraints) |
 | HARD_SWISH | [Generic](#tflite-generic-constraints), [Specific](#tflite-hard_swish-constraints) |
 | LEAKY_RELU | [Generic](#tflite-generic-constraints), [Specific](#tflite-leaky_relu-constraints) |
 | LOGISTIC | [Generic](#tflite-generic-constraints) |
 | MAXIMUM | [Generic](#tflite-generic-constraints), [Specific](#tflite-maximum-constraints) |
 | MAX_POOL_2D | [Generic](#tflite-generic-constraints), [Specific](#tflite-max_pool_2d-constraints) |
@@ -50,32 +70,34 @@
 | SPLIT | [Generic](#tflite-generic-constraints), [Specific](#tflite-split-constraints) |
 | SPLIT_V | [Generic](#tflite-generic-constraints), [Specific](#tflite-split_v-constraints) |
 | SQUEEZE | [Generic](#tflite-generic-constraints), [Specific](#tflite-squeeze-constraints) |
 | STRIDED_SLICE | [Generic](#tflite-generic-constraints), [Specific](#tflite-strided_slice-constraints) |
 | SUB | [Generic](#tflite-generic-constraints), [Specific](#tflite-sub-constraints) |
 | TANH | [Generic](#tflite-generic-constraints) |
 | TRANSPOSE_CONV | [Generic](#tflite-generic-constraints), [Specific](#tflite-transpose_conv-constraints) |
+| UNIDIRECTIONAL_SEQUENCE_LSTM | [Generic](#tflite-generic-constraints), [Specific](#tflite-unidirectional_sequence_lstm-constraints) |
 | UNPACK | [Generic](#tflite-generic-constraints) |
 
 ### TFLite Generic Constraints
 
 This is a list of constraints most NPU operators must satisfy in order to be scheduled on the NPU.
 (Operators excluded from certain constraints are shown in brackets [ ] )
 
+- All required operator attributes must be specified
 - Input(s) and Output tensors must not be dynamic - [QUANTIZE]
 - Input(s) and Output tensors must have a defined shape
 - Output tensors cannot be scalar - [QUANTIZE]
-- Scalar Input tensors are only valid for op type: ADD, EXPAND_DIMS, MAXIMUM, MEAN, MINIMUM, MUL, QUANTIZE, SPLIT, SPLIT_V, SUB
+- Scalar Input tensors are only valid for op type: ADD, ARG_MAX, EXPAND_DIMS, MAXIMUM, MEAN, MINIMUM, MUL, QUANTIZE, SPLIT, SPLIT_V, SUB
 - Input(s) and Output tensors must not be greater than 4D
-- Input(s), Output and Weight tensors must have quantization parameters - [SHAPE]
+- Input(s), Output and Weight tensors must have quantization parameters - [ARG_MAX, SHAPE]
 - Input(s), Output and Weight tensors with quantization scales must be finite
 - Input and Output tensors must have quantization scales that fit within float32 precision
 - Constant tensors should not have NoneType-values
-- Tensors must be of type: int16, int32, int8, uint8
-- Tensors which are int32 are only valid when op type is: ADD, MUL, SHAPE, SUB
+- Tensors must be of type: int16, int32, int8, uint8 - [ARG_MAX]
+- Tensors which are int32 are only valid when op type is: ADD, ARG_MAX, MUL, SHAPE, SUB
 - Tensor dimensions must be in the range [1, 65535]
 - Per-axis quantization is only supported for the following op types: CONV_2D, DEPTHWISE_CONV_2D, TRANSPOSE_CONV
 - IFM Tensor batch size must be 1 - [FULLY_CONNECTED, RESHAPE, SHAPE, SLICE, SOFTMAX, SPLIT, SPLIT_V, SQUEEZE, STRIDED_SLICE, UNPACK]
 - The fused activation function (if present) must be one of type: LOGISTIC, RELU, RELU6, RELU_N1_TO_1, TANH
 - If a fused activation function is present, the Output tensor must be one of type: int16, int8, uint8
 
 ### TFLite ABS Constraints
@@ -91,14 +113,23 @@
 
 - At least one Input's shape must match the OFM's shape
 - Both Input data types must match
 - For IFM that are signed, OFM must also be signed
 - For IFM that are unsigned, OFM must either be the same type or int32
 - Broadcasting is only allowed for rank indices with dimension 1, from either IFM1 or IFM2
 
+### TFLite ARG_MAX Constraints
+
+This is a list of constraints that the ARG_MAX operator must satisfy in order to be scheduled on the NPU.
+
+- IFM must be int8 or uint8
+- OFM must be int32 or int64
+- Operation must be performed along the depth axis
+- IFM depth must be no greater than 127
+
 ### TFLite AVERAGE_POOL_2D Constraints
 
 This is a list of constraints that the AVERAGE_POOL_2D operator must satisfy in order to be scheduled on the NPU.
 
 - Stride values for both width and height must be integer types
 - IFM and OFM data types must match
 - Kernel filter values for both width and height must be integer types
@@ -119,15 +150,15 @@
 
 ### TFLite CONV_2D Constraints
 
 This is a list of constraints that the CONV_2D operator must satisfy in order to be scheduled on the NPU.
 
 - Stride values for both width and height must be integer types
 - Dilation factor values for both width and height must be integer types
-- Stride values for height must be between 1 and 3 and for width between 1 and 4
+- Stride width must be greater than or equal to 1 and stride height must be between 1 and 3
 - Dilated kernel height must be in the range [1, 64]
 - Product of dilated kernel width and height must be in the range [1, 4096]
 - Weight tensor must be 8-bit
 - Weight tensor must be constant
 - The sum of the weights cannot exceed 8323072
 - Optional Bias tensor must be of shape: 1D
 - Optional Bias tensor must be of type: int32, int64
@@ -146,19 +177,28 @@
 - The sum of the weights cannot exceed 8323072
 - Optional Bias tensor must be of shape: 1D
 - Optional Bias tensor must be of type: int32, int64
 - Optional Bias tensor values must fit within 40-bits
 - Stride values for both width and height must be between 1 and 3
 - For depth multipliers > 1, IFM channels must be 1 and OFM channels must be equal to the depth multiplier
 
+### TFLite EXP Constraints
+
+This is a list of constraints that the EXP operator must satisfy in order to be scheduled on the NPU.
+
+- At least one Input's shape must match the OFM's shape
+- IFM and OFM data types must match
+- IFM must be int8 or int16
+
 ### TFLite EXPAND_DIMS Constraints
 
 This is a list of constraints that the EXPAND_DIMS operator must satisfy in order to be scheduled on the NPU.
 
 - Input and output quantisation must match.
+- Input and output number of elements must match.
 
 ### TFLite FULLY_CONNECTED Constraints
 
 This is a list of constraints that the FULLY_CONNECTED operator must satisfy in order to be scheduled on the NPU.
 
 - The output tensor(s) must have 2D shape
 - The IFM and OFM must have the same number of dimensions if keep_num_dims is set to true
@@ -202,24 +242,19 @@
 - Kernel filter height must be in the range [1, 256]
 - Product of kernel filter width and height must be in the range [1, 65536]
 
 ### TFLite MEAN Constraints
 
 This is a list of constraints that the MEAN operator must satisfy in order to be scheduled on the NPU.
 
-- IFM must be int8 or uint8
 - Input tensor must be at least 2D
 - Axis indices must correspond to height and width axes
-- Product of height and width must be no greater than 65536
-- Product of height and width must be no greater than 4096 when:  
-        IFM and OFM have different scale or zero point; or  
-        'keep_dims' is True
+- Product of height and width must be no greater than 4096
 - For single axis averages across the height dimension:  
-        IFM height must be no greater than 256 if the IFM and OFM scale and zero point match; otherwise  
-        IFM height must be no greater than 64 if the IFM and OFM scale or zero point do not match
+        IFM height must be no greater than 64
 
 ### TFLite MINIMUM Constraints
 
 This is a list of constraints that the MINIMUM operator must satisfy in order to be scheduled on the NPU.
 
 - At least one Input's shape must match the OFM's shape
 - IFM and OFM data types must match
@@ -247,28 +282,31 @@
 - Pad tensor must be of type: int32, int64
 
 ### TFLite RESHAPE Constraints
 
 This is a list of constraints that the RESHAPE operator must satisfy in order to be scheduled on the NPU.
 
 - Input and output quantisation must match.
+- Input and output number of elements must match.
 - Shape must be constant
 
 ### TFLite RESIZE_BILINEAR Constraints
 
 This is a list of constraints that the RESIZE_BILINEAR operator must satisfy in order to be scheduled on the NPU.
 
 - The width and height of the IFM and OFM must match one of the following criteria:  
         IFM W and H must both be 1  
         IFM must match OFM  
         W and H scaling must be equal and OFM W-1 and H-1 must be 2x/4x/8x IFM W-1 and H-1, if align_corners is True  
         W and H scaling must be equal and OFM W and H must be 2x/4x/8x IFM W and H, if align_corners is False
 - The size tensor must match the output tensor shape
 - Both align_corners and half_pixel_centers can't be True
-- Half_pixel_centers for resize bilinear requires that OFM W and H is 2x IFM W and H
+- For half_pixel_centers the width and height of the IFM and OFM must match one of the following criteria:  
+        IFM W and H are both 1  
+        OFM W and H is 2x IFM W and H
 
 ### TFLite RESIZE_NEAREST_NEIGHBOR Constraints
 
 This is a list of constraints that the RESIZE_NEAREST_NEIGHBOR operator must satisfy in order to be scheduled on the NPU.
 
 - The width and height of the IFM and OFM must match one of the following criteria:  
         IFM W and H must both be 1  
@@ -300,14 +338,15 @@
 - Only one size is allowed to be inferred
 
 ### TFLite SQUEEZE Constraints
 
 This is a list of constraints that the SQUEEZE operator must satisfy in order to be scheduled on the NPU.
 
 - Input and output quantisation must match.
+- Input and output number of elements must match.
 
 ### TFLite STRIDED_SLICE Constraints
 
 This is a list of constraints that the STRIDED_SLICE operator must satisfy in order to be scheduled on the NPU.
 
 - Exactly 4 Input tensors are required
 - Begin, End and Stride Input tensors must be constant
@@ -339,7 +378,23 @@
 - Optional Bias tensor must be of shape: 1D
 - Optional Bias tensor must be of type: int32, int64
 - Optional Bias tensor values must fit within 40-bits
 - Stride values for both width and height must be 2
 - SAME padding: OFM dimensions must equal IFM dimensions multiplied by stride
 - VALID padding: OFM dimensions must equal IFM dimensions multiplied by stride,  
         minus difference between kernel size and stride
+
+### TFLite UNIDIRECTIONAL_SEQUENCE_LSTM Constraints
+
+This is a list of constraints that the UNIDIRECTIONAL_SEQUENCE_LSTM operator must satisfy in order to be scheduled on the NPU.
+
+- IFM must be int8 or int16
+- IFM and OFM data types must match
+- IFM and OFM must have 3D shape
+- Must have 24 input tensors
+- Must have 5 intermediate tensors
+- State tensors must be variable
+- Must not use CIFG
+- Must not use Peephole
+- Must not use Projection
+- Must not use Normalisation
+- All input and recurrent weights must be available
```

### Comparing `ethos-u-vela-3.7.0/TESTING.md` & `ethos-u-vela-3.8.0/TESTING.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,32 @@
+<!--
+SPDX-FileCopyrightText: Copyright 2020, 2022-2023 Arm Limited and/or its affiliates <open-source-office@arm.com>
+
+SPDX-License-Identifier: Apache-2.0
+
+Licensed under the Apache License, Version 2.0 (the License); you may
+not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an AS IS BASIS, WITHOUT
+WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+-->
 # Vela Testing
 
 ## Tools
 
 Vela's Python codebase is PEP8 compliant with the exception of a 120 character
 line length.  The following code formatting and linting tools are run on all the
-Python files (excluding the directories `ethosu/vela/tflite/` and
-`ethosu/vela/ethos_u55_regs` because they contain auto-generated code):
+Python files (excluding the directories `ethosu/vela/tflite/`, `ethosu/vela/tosa/`,
+and `ethosu/vela/ethos_u55_regs` because they contain auto-generated code):
 
 * mypy (code linter)
 * reorder-python-import (code formatter)
 * black (code formatter)
 * flake8 (code linter)
 * pylint (code linter)
 
@@ -17,25 +34,29 @@
 This is also used to run the following test and coverage tools:
 
 * pytest (testing framework)
 * pytest-cov (code coverage plugin for pytest)
 
 ### Installation
 
-To install pre-commit, pytest and pytest-cov use the following command:
+To install the development dependencies, use the following command:
 
-```bash
-pip install pre-commit
-...
-pip install pytest
-...
-pip install pytest-cov
+``` bash
+pip install -e .[dev]
 ```
 
-The remaining tools will all be installed automatically upon first use.
+This command will install the following tools:
+
+* pytest
+* pytest-cov
+* pre-commit
+* build
+* setuptools_scm
+
+The remaining tools will all be installed automatically upon first use of pre-commit.
 
 ### Add pre-commit hook (Automatically running the tools)
 
 To support code development all the above tools can be configured to run
 automatically on `git commit` (except pytest-cov which is run on `git push`) by
 using the command:
```

### Comparing `ethos-u-vela-3.7.0/ethos_u_vela.egg-info/PKG-INFO` & `ethos-u-vela-3.8.0/ethos_u_vela.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,47 @@
 Metadata-Version: 2.1
 Name: ethos-u-vela
-Version: 3.7.0
+Version: 3.8.0
 Summary: Neural network model compiler for Arm Ethos-U NPUs
 Author-email: Arm Ltd <mlg-vela@arm.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://git.mlplatform.org/ml/ethos-u/ethos-u-vela.git/
 Keywords: ethos-u,vela compiler,tflite,npu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Compilers
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE.txt
 
+<!--
+SPDX-FileCopyrightText: Copyright 2020-2023 Arm Limited and/or its affiliates <open-source-office@arm.com>
+
+SPDX-License-Identifier: Apache-2.0
+
+Licensed under the Apache License, Version 2.0 (the License); you may
+not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an AS IS BASIS, WITHOUT
+WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+-->
 # Vela
 
 This tool is used to compile a
 [TensorFlow Lite for Microcontrollers](https://www.tensorflow.org/lite/microcontrollers)
 neural network model into an optimised version that can run on an embedded
 system containing an
 [Arm Ethos-U NPU](https://www.arm.com/products/silicon-ip-cpu).
@@ -46,16 +64,16 @@
 compiled model.
 
 The tool has limited functionality for compiling a
 [TOSA](https://git.mlplatform.org/tosa/specification.git/) neural network
 (EXPERIMENTAL).
 
 ## TensorFlow Support
-
-* Vela 3.6.0 to current supports TensorFlow 2.10
+* Vela 3.8.0 to current supports TensorFlow 2.11
+* Vela 3.6.0 to 3.7.0 supports TensorFlow 2.10
 * Vela 3.5.0 supports TensorFlow 2.9
 * Vela 3.4.0 supports TensorFlow 2.8
 * Vela 3.3.0 supports TensorFlow 2.7
 * Vela 3.1.0 to 3.2.0 supports TensorFlow 2.5
 * Vela 2.1.0 to 3.0.0 supports TensorFlow 2.4
 * Vela 2.0.0 to 2.0.1 supports TensorFlow 2.3
 * Vela 0.1.0 to 1.2.0 supports TensorFlow 2.1
@@ -64,17 +82,17 @@
 
 Vela runs on Linux and Microsoft Windows 10 operating systems.
 
 ## Prerequisites
 
 The following should be installed prior to the installation of Vela:
 
-* Python 3.7 or compatible
+* Python 3.9 or compatible
    - Development version containing the Python/C API header files
-   - e.g. `apt install python3.7-dev` or `yum install python37-devel`
+   - e.g. `apt install python3.9-dev` or `yum install python39-devel`
 * Pip3
 * A C99 capable compiler and associated toolchain
     - For Linux operating systems, a GNU toolchain is recommended.
     - For Microsoft Windows 10, Microsoft Visual C++ 14.2 Build Tools is recommended.
       See <https://wiki.python.org/moin/WindowsCompilers>
 
 ## Installation
@@ -118,25 +136,25 @@
 This is done by adding the `-e` option to the install command like so:
 
 ```bash
 pip3 install -e .
 ```
 
 If you plan to contribute to the Vela project (highly encouraged!) then it is
-recommended to install Vela along with the pre-commit tools (see
-[Vela Testing](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.7.0/TESTING.md) for more details).
+recommended to install Vela with the development dependencies (see
+[Vela Testing](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/TESTING.md) for more details).
 
 ## Running
 
 Vela is run with an input `.tflite` or `.tosa` (EXPERIMENTAL) file passed on the
 command line. This file contains the neural network to be compiled. The tool then
 outputs an optimised `.tflite` file with a `_vela` suffix in the file name, along
 with performance estimate (EXPERIMENTAL) CSV files, all to the output directory.
 It also prints a performance estimation summary back to the console, see
-[Vela Performance Estimation Summary](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.7.0/PERFORMANCE.md).
+[Vela Performance Estimation Summary](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/PERFORMANCE.md).
 
 Example usage:
 
 1) Compile the network `my_model.tflite`.  The optimised version will be output
 to `./output/my_network_vela.tflite`.
 
 ```bash
@@ -223,15 +241,15 @@
 the mlw_codec and the current version of NumPy.
 
 **Example scenario:**
 
 In the ethos-u-vela source directory, run:
 
 ```bash
-virtualenv -p 3.8 venv
+virtualenv -p 3.9 venv
 . venv/bin/activate
 pip install ethos-u-vela
 ```
 
 Next, install a different NumPy version (e.g. 1.21.3)
 
 ```bash
@@ -269,66 +287,66 @@
    in mlw_codec during the build process.
    ```
    pip install ethos-u-vela --no-build-isolation --no-cache-dir
    ```
 
 ## APIs
 
-Please see [Vela External APIs](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.7.0/API.md).
+Please see [Vela External APIs](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/API.md).
 
 ## Bug Reporting
 
-Please see [Vela Community Bug Reporting](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.7.0/BUGS.md) for a description of how to
+Please see [Vela Community Bug Reporting](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/BUGS.md) for a description of how to
 report bugs.
 
 ## Contributions
 
-Please see [Vela Contributions](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.7.0/CONTRIBUTIONS.md).
+Please see [Vela Contributions](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/CONTRIBUTIONS.md).
 
 ## Debug Database
 
-Please see [Vela Debug Database](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.7.0/DEBUG_DB.md).
+Please see [Vela Debug Database](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/DEBUG_DB.md).
 
 ## Inclusive language commitment
 
 This product conforms to Arm’s inclusive language policy and, to the best of
 our knowledge, does not contain any non-inclusive language. If you find
 something that concerns you, email terms@arm.com.
 
 ## Options
 
-Please see [Vela CLI Options](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.7.0/OPTIONS.md).  This includes a description of the
+Please see [Vela CLI Options](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/OPTIONS.md).  This includes a description of the
 system configuration file format.
 
 ## Performance
 
-Please see [Vela Performance Estimation Summary](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.7.0/PERFORMANCE.md).
+Please see [Vela Performance Estimation Summary](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/PERFORMANCE.md).
 
 ## Releases
 
-Please see [Vela Releases](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.7.0/RELEASES.md).
+Please see [Vela Releases](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/RELEASES.md).
 
 ## Resources
 
 Additional useful information:
 
 * [Arm Products: Ethos-U55 NPU](https://www.arm.com/products/silicon-ip-cpu/ethos/ethos-u55)
 * [Arm Products: Ethos-U65 NPU](https://www.arm.com/products/silicon-ip-cpu/ethos/ethos-u65)
 * [Arm Developer: Ethos-U55 NPU](https://developer.arm.com/ip-products/processors/machine-learning/arm-ethos-u/ethos-u55)
 * [Arm Developer: Ethos-U65 NPU](https://developer.arm.com/ip-products/processors/machine-learning/arm-ethos-u/ethos-u65)
 
 ## Security
 
-Please see [Vela Security](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.7.0/SECURITY.md).
+Please see [Vela Security](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/SECURITY.md).
 
 ## Supported Operators
 
-Please see [Vela Supported Operators](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.7.0/SUPPORTED_OPS.md) for the list of
+Please see [Vela Supported Operators](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/SUPPORTED_OPS.md) for the list of
 operators supported in this release.
 
 ## Testing
 
-Please see [Vela Testing](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.7.0/TESTING.md).
+Please see [Vela Testing](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/TESTING.md).
 
 ## License
 
-Vela is licensed under [Apache License 2.0](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.7.0/LICENSE.txt).
+Vela is licensed under [Apache License 2.0](https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/3.8.0/LICENSE.txt).
```

### Comparing `ethos-u-vela-3.7.0/ethos_u_vela.egg-info/SOURCES.txt` & `ethos-u-vela-3.8.0/ethos_u_vela.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 ethosu/vela/graph_optimiser_util.py
 ethosu/vela/greedy_allocation.py
 ethosu/vela/high_level_command_stream.py
 ethosu/vela/high_level_command_stream_generator.py
 ethosu/vela/high_level_command_to_npu_op.py
 ethosu/vela/hillclimb_allocation.py
 ethosu/vela/live_range.py
+ethosu/vela/lstm.py
 ethosu/vela/lut.py
 ethosu/vela/mark_tensors.py
 ethosu/vela/model_reader.py
 ethosu/vela/nn_graph.py
 ethosu/vela/npu_performance.py
 ethosu/vela/npu_serialisation.py
 ethosu/vela/numeric_util.py
@@ -84,19 +85,21 @@
 ethosu/vela/tflite_supported_operators.py
 ethosu/vela/tflite_writer.py
 ethosu/vela/tosa_graph_optimiser.py
 ethosu/vela/tosa_mapping.py
 ethosu/vela/tosa_model_semantic.py
 ethosu/vela/tosa_reader.py
 ethosu/vela/tosa_supported_operators.py
+ethosu/vela/utils.py
 ethosu/vela/vela.py
 ethosu/vela/weight_compressor.py
 ethosu/vela/ethos_u55_regs/__init__.py
 ethosu/vela/ethos_u55_regs/ethos_u55_regs.py
 ethosu/vela/test/test_architecture_allocator.py
+ethosu/vela/test/test_build.py
 ethosu/vela/test/test_compiler_driver.py
 ethosu/vela/test/test_fp_math.py
 ethosu/vela/test/test_graph_optimiser.py
 ethosu/vela/test/test_hillclimb_allocation.py
 ethosu/vela/test/test_live_range.py
 ethosu/vela/test/test_lut.py
 ethosu/vela/test/test_model_reader.py
```

### Comparing `ethos-u-vela-3.7.0/ethosu/config_files/Arm/vela.ini` & `ethos-u-vela-3.8.0/ethosu/config_files/Arm/vela.ini`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/mlw_codec/makefile` & `ethos-u-vela-3.8.0/ethosu/mlw_codec/makefile`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/mlw_codec/mlw_codecmodule.c` & `ethos-u-vela-3.8.0/ethosu/mlw_codec/mlw_codecmodule.c`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/mlw_codec/mlw_common.h` & `ethos-u-vela-3.8.0/ethosu/mlw_codec/mlw_common.h`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/mlw_codec/mlw_decode.c` & `ethos-u-vela-3.8.0/ethosu/mlw_codec/mlw_decode.c`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/mlw_codec/mlw_decode.h` & `ethos-u-vela-3.8.0/ethosu/mlw_codec/mlw_decode.h`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/mlw_codec/mlw_encode.c` & `ethos-u-vela-3.8.0/ethosu/mlw_codec/mlw_encode.c`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/mlw_codec/mlw_encode.h` & `ethos-u-vela-3.8.0/ethosu/mlw_codec/mlw_encode.h`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/mlw_codec/mlw_main.c` & `ethos-u-vela-3.8.0/ethosu/mlw_codec/mlw_main.c`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/mlw_codec/test/test_mlw_codec.py` & `ethos-u-vela-3.8.0/ethosu/mlw_codec/test/test_mlw_codec.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/__init__.py` & `ethos-u-vela-3.8.0/ethosu/vela/__init__.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/__main__.py` & `ethos-u-vela-3.8.0/ethosu/vela/__main__.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/_version.py` & `ethos-u-vela-3.8.0/ethosu/vela/_version.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/api.py` & `ethos-u-vela-3.8.0/ethosu/vela/api.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/architecture_allocator.py` & `ethos-u-vela-3.8.0/ethosu/vela/architecture_allocator.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/architecture_features.py` & `ethos-u-vela-3.8.0/ethosu/vela/architecture_features.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/cascade_builder.py` & `ethos-u-vela-3.8.0/ethosu/vela/cascade_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,17 +184,14 @@
             ops_in_best_cascade = [op]
             # Get the size of the weight buffer(s)
             weight_buffer = sum(tens.storage_size() for tens in ref_cost[op].buffered_weight_tensors)
 
             # The first IFM needs to be stored in full
             cascade_ifm_size = op.ifm_size_in_bytes() if not self.spilling else 0
 
-            # Add non-local memory usage
-            cascade_ifm_size += self.non_local_mem_usage.get(op, 0)
-
             # Sum of all intermediate cascade buffers (including weight buffers)
             cascade_buffers = weight_buffer
             # Best cascade size - Initially it's the fallback cost of the first Op in the cascade
             best_cascade_size = self._estimate_sram_usage(op, fallback_cost[op])
 
             # Op is the producer of the OFM consumed by the next Op to consider
             producer = op
@@ -244,24 +241,27 @@
                         break
                     else:
                         # Any addition to the cascade that fits is the new best cascade for Dedicated SRAM
                         ops_in_best_cascade = [op for op in ops_in_cascade]
                         best_cascade_size = cascade_buffers
 
                 else:
-                    # Calculate the total size of the current cascade
-                    cascade_size = cascade_ifm_size + cascade_buffers + op_full_ofm
+                    # Calculate the total size of the current cascade including non local mem usage
+                    cascade_size = (
+                        cascade_ifm_size + cascade_buffers + op_full_ofm + self.non_local_mem_usage.get(op, 0)
+                    )
 
                     # Determine if cascading search should stop
                     if (
                         uncascaded_sram_usage < peak_sram_usage
                         and best_cascade_size < peak_sram_usage
                         or (cascade_ifm_size + cascade_buffers) > best_cascade_size
                     ):
-                        # Both the existing cascade and current Op fits
+                        # Both the existing cascade and current Op fits or
+                        # not possible to reduce cascade size any further
                         break
 
                     """
                     One of two conditions will update the best cascade:
 
                     - cascade_size < best_cascade_size or
                     - cascade_size < uncascaded_sram_usage
@@ -302,15 +302,15 @@
 
                     (FM + roll buffer + roll buffer + FM) <  (FM + roll buffer + FM) or
                     (FM + roll buffer + roll buffer + FM) <  (FM + FM + FM)
 
                     hence, better to choose Cascade OP1-OP3 in this case.
                     """
                     if cascade_size < best_cascade_size or cascade_size < uncascaded_sram_usage:
-                        best_cascade_size = cascade_ifm_size + cascade_buffers + op_full_ofm
+                        best_cascade_size = cascade_size
                         ops_in_best_cascade = [op for op in ops_in_cascade]
 
                 producer = current_op
 
             if len(ops_in_best_cascade) > 1:
                 # A cascade was created - assign cascade and ref_cost to all of the Ops
                 cascade_end = cascade_start + (len(ops_in_best_cascade) - 1)
@@ -322,17 +322,23 @@
                     cost[cascaded_op].cascade = cascade_end
                     if prev_op:
                         rolling_buffer_shape, _ = buffers.get_buffer(prev_op, cascaded_op, ref_cost)
                         buffers_in_cascade[cascaded_op] = rolling_buffer_shape
 
                     prev_op = cascaded_op
 
-                # Create a CascadeInfo for the cascade
+                # Create a CascadeInfo for the cascade, only store the actual size used by
+                # the cascade so non local usage is removed. This is done in order to be
+                # able to calculate the correct non local usage in the scheduler when
+                # optimizing the sub schedules.
                 cascade_map[cascade_end] = CascadeInfo(
-                    cascade_start, cascade_end, buffers_in_cascade, best_cascade_size
+                    cascade_start,
+                    cascade_end,
+                    buffers_in_cascade,
+                    best_cascade_size - self.non_local_mem_usage.get(op, 0),
                 )
                 if not self.spilling:
                     # Update peak memory usage
                     peak_sram_usage = max(best_cascade_size, peak_sram_usage)
             else:
                 # Assign fallback cost to the initial Op
                 cost[op] = fallback_cost[op]
```

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/compiler_driver.py` & `ethos-u-vela-3.8.0/ethosu/vela/compiler_driver.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from .operation import Op
 from .rewrite_graph import verify_graph_health
 from .rewrite_graph import visit_graph_post_order
 from .scheduler import OptimizationStrategy
 from .tensor import MemArea
 from .tensor import MemType
 from .tensor import Tensor
+from .utils import progress_print
 
 
 class CompilerOptions:
     """Set of options to change compiler behaviour - verbosity, targets, turning off passes.
 
     Note the difference between ArchitectureFeatures and CompilerOptions
     - ArchitectureFeatures is for changing the Ethos-U and system architecture
@@ -58,14 +59,15 @@
         verbose_tensor_format=False,
         verbose_allocation=False,
         verbose_high_level_command_stream=False,
         verbose_register_command_stream=False,
         verbose_operators=False,
         verbose_weights=False,
         verbose_performance=False,
+        verbose_progress=False,
         show_cpu_operations=False,
         tensor_allocator=TensorAllocator.Greedy,
         timing=False,
         force_symmetric_int_weights=False,
         output_dir="outputs",
         cpu_tensor_alignment=Tensor.AllocationQuantum,
         hillclimb_max_iterations=None,
@@ -78,14 +80,15 @@
         self.verbose_tensor_format = verbose_tensor_format
         self.verbose_allocation = verbose_allocation
         self.verbose_high_level_command_stream = verbose_high_level_command_stream
         self.verbose_register_command_stream = verbose_register_command_stream
         self.verbose_operators = verbose_operators
         self.verbose_weights = verbose_weights
         self.verbose_performance = verbose_performance
+        self.verbose_progress = verbose_progress
         self.show_cpu_operations = show_cpu_operations
         self.tensor_allocator = tensor_allocator
         self.timing = timing
         self.force_symmetric_int_weights = force_symmetric_int_weights
         self.output_dir = output_dir
         self.cpu_tensor_alignment = cpu_tensor_alignment
         self.hillclimb_max_iterations = hillclimb_max_iterations
@@ -150,38 +153,45 @@
                 f" Target = {scheduler_options.optimization_sram_limit} Bytes,"
                 f" Actual = {sram_usage} Bytes"
             )
 
 
 def compiler_driver(nng, arch, options, scheduler_options, network_type, output_basename):
     assert verify_graph_health(nng)
+    verbose_progress = scheduler_options.verbose_progress
 
     # Pre-optimisation operator tracking
     for sg in nng.subgraphs:
         visit_graph_post_order(sg.output_tensors, arch, [], [_record_operator])
 
+    progress_print(verbose_progress, "Performing graph optimisation")
     nng = graph_optimiser.optimise_graph(
         nng, arch, network_type, options.verbose_graph, options.force_symmetric_int_weights
     )
     assert verify_graph_health(nng)
 
     if options.verbose_quantization:
         nng.print_graph_with_tensor_quantization()
 
+    progress_print(verbose_progress, "Defining tensor purpose")
     nng = mark_tensors.mark_tensor_purpose(nng, arch, options.verbose_tensor_purpose)
     assert verify_graph_health(nng)
+
+    progress_print(verbose_progress, "Performing pass packing")
     pass_packing.pack_into_passes(nng, arch, options.verbose_packing)
     assert verify_graph_health(nng)
 
+    progress_print(verbose_progress, "Extracting npu subgraphs")
     extract_npu_subgraphs.extract_npu_subgraphs(nng, arch)
 
     assert verify_graph_health(nng)
     if options.timing:
         start = time.time()
 
+    progress_print(verbose_progress, "Scheduling passes")
     # Run the scheduler
     scheduler.schedule_passes(nng, arch, options, scheduler_options)
     _check_schedule(nng, arch, scheduler_options)
 
     if options.timing:
         stop = time.time()
         print("Scheduling took %f s" % (stop - start))
@@ -195,24 +205,26 @@
     scratch_tens = None
     scratch_fast_tens = None
     flash_tens = None
 
     # Create list of NPU subgraphs with same order as the list of all subgraphs
     npu_subgraphs = [sg for sg in nng.subgraphs if sg.placement == PassPlacement.Npu]
 
+    progress_print(verbose_progress, "Calculating live ranges for constant NPU tensors")
     # Calculate live ranges for all constant Npu tensors, in permanent storage
     for sg in npu_subgraphs:
         lr_graph_flash = live_range.create_linear_live_range_graph(
             sg,
             permanent_storage,
             MemType.Permanent_NPU,
             lr_graph=lr_graph_flash,
         )
 
     if npu_subgraphs:
+        progress_print(verbose_progress, "Allocating NPU constant tensors to the first NPU subgraph")
         # Allocate all Npu constant tensors to the first Npu subgraph since it is
         # processed first during serialization into tensors
         first_npu_sg = npu_subgraphs[0]
         tensor_allocation.allocate_tensors(
             nng,
             first_npu_sg,
             arch,
@@ -221,14 +233,15 @@
             tensor_allocator=TensorAllocator.LinearAlloc,
             verbose_allocation=options.verbose_allocation,
             lr_graph=lr_graph_flash,
         )
 
     root_sg = nng.get_root_subgraph()
 
+    progress_print(verbose_progress, "Generating command stream")
     # Generate command streams and serialise Npu-ops into tensors
     for sg in npu_subgraphs:
         high_level_command_stream_generator.generate_high_level_command_stream_for_schedule(
             nng, sg, arch, options.verbose_high_level_command_stream
         )
         lut.optimize_high_level_cmd_stream(sg, arch)
         high_level_command_to_npu_op.generate_register_command_stream_for_sg(
@@ -245,23 +258,24 @@
 
     # Set Scratch and Fast_scratch Tensor size
     if scratch_tens is not None:
         scratch_tens.set_all_shapes([root_sg.memory_used_per_type.get(MemType.Scratch, 0)])
     if scratch_fast_tens is not None:
         scratch_fast_tens.set_all_shapes([root_sg.memory_used_per_type.get(MemType.Scratch_fast, 0)])
 
+    progress_print(verbose_progress, "Allocating CPU constant tensors")
     # Allocate all Cpu constant tensors, this is done last because the Npu-ops
     # have to be serialized into flash and scratch tensors first
     tensor_allocation.allocate_tensors(
         nng,
         root_sg,
         arch,
         permanent_storage,
         set((MemType.Permanent_CPU,)),
         tensor_allocator=TensorAllocator.LinearAlloc,
         verbose_allocation=options.verbose_allocation,
         cpu_tensor_alignment=options.cpu_tensor_alignment,
     )
-
+    progress_print(verbose_progress, "Calculating new performance for the network")
     npu_performance.calc_new_performance_for_network(
         nng, arch, network_type, options.verbose_performance, output_basename
     )
```

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/data_type.py` & `ethos-u-vela-3.8.0/ethosu/vela/data_type.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/debug_database.py` & `ethos-u-vela-3.8.0/ethosu/vela/debug_database.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/driver_actions.py` & `ethos-u-vela-3.8.0/ethosu/vela/driver_actions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/errors.py` & `ethos-u-vela-3.8.0/ethosu/vela/errors.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/ethos_u55_regs/ethos_u55_regs.py` & `ethos-u-vela-3.8.0/ethosu/vela/ethos_u55_regs/ethos_u55_regs.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/extract_npu_subgraphs.py` & `ethos-u-vela-3.8.0/ethosu/vela/extract_npu_subgraphs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright 2020-2022 Arm Limited and/or its affiliates <open-source-office@arm.com>
+# SPDX-FileCopyrightText: Copyright 2020-2023 Arm Limited and/or its affiliates <open-source-office@arm.com>
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 # Licensed under the Apache License, Version 2.0 (the License); you may
 # not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -246,15 +246,15 @@
                     rewrite_tensor_npu_producer_cpu_consumers(
                         tens, call_pass[curr_sg], startup_init_passes[curr_sg], curr_sg, orig_sg, subgraph_for_pass
                     )
 
         for tens in curr_sg.output_tensors:
             # ofm can depend on multiple ops. These ops can be divided into different NPU
             # nodes due to CPU nodes. If that is the case the ofm must be NHWC.
-            tens.needs_linear_format = True
+            tens.force_linear_format = True
 
     return new_subgraphs
 
 
 def extract_npu_subgraphs(nng, arch):
 
     nng.refresh_after_modification()
```

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/fp_math.py` & `ethos-u-vela-3.8.0/ethosu/vela/fp_math.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/graph_optimiser.py` & `ethos-u-vela-3.8.0/ethosu/vela/graph_optimiser.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/greedy_allocation.py` & `ethos-u-vela-3.8.0/ethosu/vela/greedy_allocation.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/high_level_command_stream.py` & `ethos-u-vela-3.8.0/ethosu/vela/high_level_command_stream.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright 2020-2022 Arm Limited and/or its affiliates <open-source-office@arm.com>
+# SPDX-FileCopyrightText: Copyright 2020-2023 Arm Limited and/or its affiliates <open-source-office@arm.com>
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 # Licensed under the Apache License, Version 2.0 (the License); you may
 # not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -289,7 +289,23 @@
         return "<DMA: in=%s, out=%s, box=%s>" % (self.in_tensor.name, self.out_tensor.name, self.box)
 
     __repr__ = __str__
 
     def get_operation_count(self):
         # returns numpy array of (DPU blocks, dma_ops)
         return np.array((0, 1))
+
+
+class NOP(Command):
+    def __init__(self, ps, in_tensor, out_tensor):
+        self.ps = ps
+        self.in_tensor = in_tensor
+        self.out_tensor = out_tensor
+
+    def __str__(self):
+        return f"<NOP: in={self.in_tensor.name}, out={self.out_tensor.name}>"
+
+    __repr__ = __str__
+
+    def get_operation_count(self):
+        # returns numpy array of (DPU blocks, dma_ops)
+        return np.array((0, 0))
```

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/high_level_command_stream_generator.py` & `ethos-u-vela-3.8.0/ethosu/vela/high_level_command_stream_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright 2020-2022 Arm Limited and/or its affiliates <open-source-office@arm.com>
+# SPDX-FileCopyrightText: Copyright 2020-2023 Arm Limited and/or its affiliates <open-source-office@arm.com>
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 # Licensed under the Apache License, Version 2.0 (the License); you may
 # not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -14,14 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # Description:
 # Generate a high-level command stream from a schedule
 from .high_level_command_stream import Box
 from .high_level_command_stream import DMA
+from .high_level_command_stream import NOP
 from .high_level_command_stream import NpuStripe
 from .numeric_util import round_up_divide
 from .operation import create_activation_function
 from .operation import NpuBlockType
 from .operation import Op
 from .shape4d import Shape4D
 from .tensor import TensorPurpose
@@ -29,14 +30,27 @@
 
 def dma_if_necessary(ps, box, tensor):
     src_tensor = tensor.src_tensor
     if src_tensor and tensor.mem_area != src_tensor.mem_area:
         yield DMA(ps, src_tensor, tensor, box)
 
 
+def dma_feature_map_if_necessary(ps, src_tensor, dst_tensor):
+    box = Box([0] * len(src_tensor.shape), list(src_tensor.shape))
+    src_addr = src_tensor.address_for_coordinate(box.start_coord)
+    dst_addr = dst_tensor.address_for_coordinate(box.start_coord)
+
+    if src_addr != dst_addr or src_tensor.mem_area != dst_tensor.mem_area:
+        yield DMA(ps, src_tensor, dst_tensor, box)
+    else:
+        # Source and destination is the same so no need for a DMA transaction
+        # Create a NOP for visibility when printing the high_level_command_stream
+        yield NOP(ps, src_tensor, dst_tensor)
+
+
 def generate_high_level_command_stream_for_schedule(nng, sg, arch, verbose_high_level_command_stream):
     res = []
     # sg.sched_ops are ordered by execution
     processed_cascades = set()
     for sched_op in sg.sched_ops:
         op_info = sg.schedule.cost_map[sched_op]
         if op_info.cascade in processed_cascades:
@@ -162,29 +176,29 @@
                         ifm.shape,
                         npu_block_type,
                         write_offset.as_list(),
                         k_dilated_height,
                         read_offsets[0],
                         read_shapes[0],
                         upscaling,
-                        op.type,
+                        sched_op.op_type,
                     )
                 # Calculate IFM2 input box based on the OFM box
                 if ifm2:
                     ifm2_box, pad_top, pad_bottom = ofm_box.transform_with_strides_and_skirt(
                         strides,
                         skirt,
                         ifm2.shape,
                         npu_block_type,
                         write_offset.as_list(),
                         k_dilated_height,
                         read_offsets[1],
                         read_shapes[1],
                         upscaling,
-                        op.type,
+                        sched_op.op_type,
                     )
 
                 ifm_required = ifm_box
                 # Get the Op that produces this Op's IFM data - only applicable within cascades
                 if producer_op:
                     assert op_info.cascade != 0
                     assert op_info.cascade == schedule.cost_map[producer_op].cascade
@@ -220,25 +234,28 @@
                 # Should only be done once per loop but not before weights above
                 if parent_op.activation_lut and not lut_dma_done:
                     lut_tensor = [tens for tens in parent_op.inputs if tens.purpose == TensorPurpose.LUT][0]
                     lut_box = Box([0] * len(lut_tensor.shape), list(lut_tensor.shape))
                     lut_dma_done = True
                     yield from dma_if_necessary(sched_op.parent_ps, lut_box, lut_tensor)
 
-                yield NpuStripe(
-                    sched_op.parent_ps,
-                    block_config.old_style_representation(),
-                    is_first_h_stripe,
-                    is_last_h_stripe,
-                    ifm_tensor,
-                    ifm_box,
-                    ofm_tensor,
-                    ofm_box,
-                    weight_tensor,
-                    weight_box,
-                    scale_tensor,
-                    ifm2_tensor=ifm2_tensor,
-                    ifm2_box=ifm2_box,
-                    pad_top=pad_top,
-                    pad_bottom=pad_bottom,
-                    reversed_operands=sched_op.reversed_operands,
-                )
+                if parent_op.type == Op.Memcpy:
+                    yield from dma_feature_map_if_necessary(sched_op.parent_ps, ifm_tensor, ofm_tensor)
+                else:
+                    yield NpuStripe(
+                        sched_op.parent_ps,
+                        block_config.old_style_representation(),
+                        is_first_h_stripe,
+                        is_last_h_stripe,
+                        ifm_tensor,
+                        ifm_box,
+                        ofm_tensor,
+                        ofm_box,
+                        weight_tensor,
+                        weight_box,
+                        scale_tensor,
+                        ifm2_tensor=ifm2_tensor,
+                        ifm2_box=ifm2_box,
+                        pad_top=pad_top,
+                        pad_bottom=pad_bottom,
+                        reversed_operands=sched_op.reversed_operands,
+                    )
```

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/high_level_command_to_npu_op.py` & `ethos-u-vela-3.8.0/ethosu/vela/high_level_command_to_npu_op.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,21 +50,23 @@
 from .data_type import DataType
 from .debug_database import DebugDatabase
 from .errors import UnsupportedFeatureError
 from .ethos_u55_regs.ethos_u55_regs import resampling_mode
 from .high_level_command_stream import Box
 from .high_level_command_stream import Command
 from .high_level_command_stream import DMA
+from .high_level_command_stream import NOP
 from .high_level_command_stream import NpuStripe
 from .numeric_util import quantise_float32
 from .numeric_util import round_up
 from .operation import NpuBlockType
 from .operation import Op
 from .operation import Operation
 from .operation import Padding
+from .operation import RoundingMode
 from .register_command_stream_generator import generate_command_stream
 from .register_command_stream_util import BASE_PTR_INDEX_MEM2MEM
 from .register_command_stream_util import to_npu_kernel
 from .register_command_stream_util import UNARY_ELEMWISE_OPS
 from .shape4d import Shape4D
 from .tensor import MemType
 from .tensor import Tensor
@@ -108,14 +110,22 @@
 resampling_mode_inv_map = {
     resampling_mode.NONE: NpuResamplingMode.NONE,
     resampling_mode.NEAREST: NpuResamplingMode.NEAREST,
     resampling_mode.TRANSPOSE: NpuResamplingMode.TRANSPOSE,
 }
 
 
+rounding_mode_map = {
+    RoundingMode.TFLite: NpuRoundingMode.TFL,
+    RoundingMode.ToZero: NpuRoundingMode.TRUNCATE,
+    RoundingMode.HalfUp: NpuRoundingMode.NATURAL,
+    RoundingMode.AwayZero: NpuRoundingMode.NATURAL,
+}
+
+
 def ifm_ifm2_correct_order(ifm_shape: Shape4D, ifm2_shape: Shape4D) -> bool:
 
     if ifm_shape is None:
         # Scalar needs to be in IFM2
         return False
     if ifm2_shape is None:
         return True
@@ -129,27 +139,27 @@
 
 def get_rounding_mode(op: Operation, fused_quantize: bool) -> NpuRoundingMode:
     """Specifies type of rounding to be used"""
     rounding_mode = NpuRoundingMode.TFL
     if op.type.is_resize_op():
         rounding_mode = NpuRoundingMode.NATURAL
     elif (
-        op.type.npu_block_type in (NpuBlockType.ConvolutionMxN, NpuBlockType.ConvolutionDepthWise)
+        op._original_type.npu_block_type in (NpuBlockType.ConvolutionMxN, NpuBlockType.ConvolutionDepthWise)
         and op.ifm.dtype == DataType.int16
     ):
         rounding_mode = NpuRoundingMode.NATURAL
     elif (
         not fused_quantize
         and op.type.is_avgpool_op()
         and op.memory_function == Op.ConcatSliceWrite
         and op.kernel.elements_wh() == 1
     ):
         rounding_mode = NpuRoundingMode.NATURAL
     if op.rounding_mode is not None:
-        rounding_mode = op.rounding_mode
+        rounding_mode = rounding_mode_map[op.rounding_mode]
     return rounding_mode
 
 
 def create_padding(cmd: NpuStripe, primary_op: Operation, npu_op: NpuBlockOperation) -> NpuPadding:
     if primary_op.type.npu_block_type == NpuBlockType.VectorProduct:
         return NpuPadding(top=0, left=0, bottom=0, right=0)
     top, left, bottom, right = primary_op.attrs["explicit_padding"]
@@ -293,18 +303,29 @@
     return block.depth
 
 
 def use_zero_point_0(ps, tens: Tensor, is_ifm_tensor: bool) -> bool:
     """Checks if quantization should use 0 as zero point"""
     if tens.dtype == DataType.int32 and is_ifm_tensor:
         return True
-    # Force zero point to 0 for ResizeBilinear when converting to a DepthwiseConv since the reference kernel
-    # will ignore the zero point.
-    if ps.primary_op.original_type == Op.ResizeBilinear and ps.primary_op.type == Op.DepthwiseConv2DBias:
-        return True
+    if ps.primary_op.rounding_mode == RoundingMode.AwayZero:
+        if ps.primary_op.original_type == Op.ResizeBilinear and ps.primary_op.type == Op.DepthwiseConv2DBias:
+            # Force zero point to 0 for ResizeBilinear operators converted to a DepthwiseConv with rounding away from
+            # zero. This is because the reference kernel ignores the zero points.
+            return True
+        if (
+            not is_ifm_tensor
+            and ps.primary_op.original_type == Op.AvgPool
+            and ps.primary_op.attrs.get("padding", None) == Padding.EXPLICIT
+            and ps.primary_op.type == Op.DepthwiseConv2DBias
+        ):
+            # Force zero point to 0 for the OFM of AvgPool operators that have been combined with a previous PAD
+            # operator and converted to a DepthwiseConv with rounding away from zero. This is because the zero point
+            # will already have been applied in the Bias.
+            return True
     if ps.primary_op.type not in (Op.AvgPool, Op.CLZ, Op.SHL) and not ps.primary_op.type.is_resize_op():
         return False
     if ps.primary_op.type == Op.AvgPool and ps.primary_op.explicit_scaling:
         return False
     fused_quantize = any(op.type == Op.Quantize for op in ps.ops)
     forced_ofm_quantization = ps.primary_op.forced_output_quantization
     use_0 = (
@@ -623,15 +644,16 @@
                 if core == 0:
                     weight_range = cmd.in_tensor.encoded_ranges[key]
                     src_addr = cmd.in_tensor.address + weight_range.offset
                     dest_addr = cmd.out_tensor.address
     else:
         src_addr = cmd.in_tensor.address_for_coordinate(cmd.box.start_coord)
         dest_addr = cmd.out_tensor.address_for_coordinate(cmd.box.start_coord)
-        sz = cmd.in_tensor.address_for_coordinate(cmd.box.end_coord, is_top_box=True) - src_addr
+        # DMA must use 16 bytes alignment (tensors are always aligned but the sz calculation uses actual size)
+        sz = round_up(cmd.in_tensor.address_for_coordinate(cmd.box.end_coord, is_top_box=True) - src_addr, 16)
     src = NpuAddressRange(src_region, int(src_addr), int(sz))
     dest = NpuAddressRange(dest_region, int(dest_addr), int(sz))
     return NpuDmaOperation(src, dest)
 
 
 def convert_command_to_npu_op(cmd: Command, arch: ArchitectureFeatures) -> NpuOperation:
     """Converts the high level command to NpuOperation"""
@@ -659,14 +681,17 @@
     """Generates command stream for the subgraph, adds it to sg.register_command_stream"""
     # Convert high level command stream to list of NpuOperation
     npu_op_list = []
     npu_op_to_cmd = dict()  # map from npu op to high level command
     for cmd in sg.high_level_command_stream:
         if isinstance(cmd, NpuStripe) and cmd.ps.npu_block_type == NpuBlockType.Default:
             print("Warning: Skipping register command stream generation for", cmd.ps)
+        elif isinstance(cmd, NOP):
+            # NOP should not generate anything
+            continue
         else:
             npu_op = convert_command_to_npu_op(cmd, arch)
             npu_op_list.append(npu_op)
             npu_op_to_cmd[npu_op] = cmd
     mem_limits = get_mem_limits_for_regions(arch)
     # Generate register commands
     if len(sg.high_level_command_stream) > 0:
```

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/hillclimb_allocation.py` & `ethos-u-vela-3.8.0/ethosu/vela/hillclimb_allocation.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/live_range.py` & `ethos-u-vela-3.8.0/ethosu/vela/live_range.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 import numpy as np
 
 from .operation import Op
 from .tensor import MemArea
 from .tensor import MemType
 from .tensor import Tensor
 from .tensor import TensorPurpose
+from .utils import progress_print
 
 
 class LiveRange:
     def __init__(self, tens, alignment):
         self.tensors = []  # Tensors that are assigned to the same LiveRange will be allocated to the same address
         self.start_time = 99999999999
         self.end_time = -1
@@ -136,23 +137,24 @@
     def fuse_ranges(self, in_tens, out_tens):
         live_range = self.get_or_create_range(in_tens)
         assert out_tens not in self.ranges, out_tens
         live_range.add_tensor(out_tens)
         self.ranges[out_tens] = live_range
         return live_range
 
-    def update_endtime(self):
-        self.end_time = self.current_time
-        return self.end_time + 1
+    def get_endtime(self):
+        # op_length is 1 so max end time for lr is current + 1
+        return self.current_time + 1
 
     def get_temporal_memory_usage(self, target_mem_area):
-        usage = np.zeros(self.update_endtime(), dtype=np.int32)
+        usage = np.zeros(self.get_endtime() + 1, dtype=np.int32)
         for lr in self.lrs:
             if lr.mem_area == target_mem_area:
                 # End time is inclusive
+                assert lr.end_time <= self.get_endtime() + 1
                 usage[lr.start_time : lr.end_time + 1] += lr.size
 
         return usage
 
 
 def tensor_should_be_ignored(tens, target_mem_area, target_mem_type_set):
     if tens.purpose == TensorPurpose.Virtual:
@@ -161,52 +163,58 @@
         return False
     if tens.mem_area != target_mem_area or tens.mem_type not in target_mem_type_set:
         return True
     return False
 
 
 def _get_ifm_to_fuse(sched_op, target_mem_area=None, target_mem_type_set=None):
-    def _tensor_should_be_ignored(tens):
-        if tens.ifm_write_protected:
-            return True
-        return tensor_should_be_ignored(tens, target_mem_area, target_mem_type_set)
-
-    # Check if possible to merge ifm/ofm live ranges of elementwise op
     ifm_tens = None
-    if sched_op.op_type.is_elementwise_op():
-        elem_op = sched_op.parent_op
-        if not _tensor_should_be_ignored(elem_op.ofm):
+    elem_op = sched_op.parent_op
+    if sched_op.op_type.is_elementwise_op() and elem_op.memory_function is not Op.VariableTensorWrite:
+        # Check if possible to merge ifm/ofm live ranges of elementwise op
+        if not tensor_should_be_ignored(elem_op.ofm, target_mem_area, target_mem_type_set):
             # Check if overwriting the inputs can be allowed
             OpShapeTens = namedtuple("OpShapeTens", ["op_shape", "tens"])
             outp = OpShapeTens(elem_op.ofm_shapes[0], elem_op.ofm)
             inps = []
             if elem_op.ifm is not None:
                 inps.append(OpShapeTens(elem_op.ifm_shapes[0], elem_op.ifm))
             if elem_op.ifm2 is not None:
                 inps.append(OpShapeTens(elem_op.ifm_shapes[1], elem_op.ifm2))
-
             # find an input tensor that can be overwritten by the output
             for inp in inps:
                 if (
                     # check op input and output shapes allow overlapping
                     inp.op_shape == outp.op_shape
                     # check input tensor is valid
                     and inp.tens is not None
                     and inp.tens.shape != []
-                    and not _tensor_should_be_ignored(inp.tens)
+                    and not inp.tens.ifm_write_protected
+                    and not tensor_should_be_ignored(inp.tens, target_mem_area, target_mem_type_set)
                     # check input and output tensors are compatible
                     and inp.tens.format == outp.tens.format
                     and inp.tens.dtype == outp.tens.dtype
                     # check input tensor only has one consumer
                     and len(inp.tens.consumer_list) == 1
                     # check output tensor only has one producer
                     and len(outp.tens.ops) == 1
                 ):
                     ifm_tens = inp.tens
                     break
+    elif sched_op.op_type == Op.Memcpy:
+        # Check if possible to merge ifm/ofm live ranges of dma op
+        dma_op = sched_op.parent_op
+        ifm = dma_op.ifm
+        ofm = dma_op.ofm
+        if not (
+            tensor_should_be_ignored(ifm, target_mem_area, target_mem_type_set)
+            or tensor_should_be_ignored(ofm, target_mem_area, target_mem_type_set)
+        ):
+            # Currently DMA only used when bypassing memory only ops so ok to reuse ifm
+            ifm_tens = ifm
 
     return ifm_tens
 
 
 def ofm_can_reuse_ifm(sched_op, target_mem_area=None, target_mem_type_set=None):
     ifm = _get_ifm_to_fuse(sched_op, target_mem_area, target_mem_type_set)
     return ifm is not None
@@ -220,23 +228,25 @@
 
 def extract_live_ranges_from_cascaded_passes(
     sg,
     target_mem_area,
     target_mem_type_set,
     lr_graph=None,
     cpu_tensor_alignment=Tensor.AllocationQuantum,
+    verbose_progress: bool = False,
 ):
     if lr_graph is None:
         lr_graph = LiveRangeGraph()
 
     if sg in lr_graph.processed_subgraphs:
         # if subgraph has been processed already, return the lr_graph as is
         return lr_graph
 
-    for cps in sg.cascaded_passes:
+    for index, cps in enumerate(sg.cascaded_passes):
+        progress_print(verbose_progress, "Processing cascaded pass", index, sg.cascaded_passes)
         cps.time = lr_graph.current_time
 
         time_for_pass = cps.time
 
         for tens in cps.inputs:
             if tensor_should_be_ignored(tens, target_mem_area, target_mem_type_set):
                 continue
@@ -247,51 +257,48 @@
         op_subgraph = op.attrs.get("subgraph", None) if op else None
 
         if op_subgraph is not None and MemType.Permanent_CPU not in target_mem_type_set:
             if op.type == Op.CustomNpuOp:
                 # If the primary-op is an NpuOp that means this is where an Npu subgraph
                 # is called. Go into said subgraph and extract live ranges before continuing.
                 # Use default allocation alignment of 16 for Npu tensors
-                lr_graph = _extract_live_ranges_from_schedule(
+                lr_graph = extract_live_ranges_from_schedule(
                     op_subgraph, target_mem_area, target_mem_type_set, lr_graph
                 )
             else:
                 # The op has one or more subgraphs in it (a typical op is the While op)
                 # Go into all subgraphs and extract live ranges before continuing.
                 for op_sg in op_subgraph:
                     lr_graph = extract_live_ranges_from_cascaded_passes(
                         op_sg, target_mem_area, target_mem_type_set, lr_graph, cpu_tensor_alignment
                     )
             # Set the new time after handling the Npu subgraph
+            # current time is updated in subgraph path so do not tick the time
             time_for_pass = lr_graph.current_time
             cps.time = time_for_pass
+        else:
+            lr_graph.current_time += 2
 
         for tens in cps.intermediates + cps.outputs:
             if tensor_should_be_ignored(tens, target_mem_area, target_mem_type_set):
                 continue
             rng = lr_graph.get_or_create_range(tens, cpu_tensor_alignment)
             rng.mark_usage(time_for_pass)
 
-        lr_graph.current_time += 2
-
-    end_time = 0
-    for rng in lr_graph.ranges.values():
-        # Find the maximum end time of all live-ranges in the graph
-        end_time = max(end_time, rng.end_time)
-
+    time_to_set = lr_graph.current_time
     for tens in sg.output_tensors:
         if tensor_should_be_ignored(tens, target_mem_area, target_mem_type_set):
             continue
         rng = lr_graph.get_or_create_range(tens, cpu_tensor_alignment)
-        rng.mark_usage(end_time)
+        rng.mark_usage(time_to_set)
 
     # Variable tensor live-range is for entire inference
     for tens, rng in lr_graph.ranges.items():
         if tens.is_variable:
-            rng.mark_usage(0, end_time + 1)
+            rng.mark_usage(0, time_to_set + 1)
 
     # Add subgraph to set of processed subgraphs
     lr_graph.processed_subgraphs.add(sg)
     return lr_graph
 
 
 def create_linear_live_range_graph(sg, target_mem_area, target_mem_type_set, lr_graph):
@@ -312,17 +319,18 @@
                 rng = lr_graph.get_or_create_range(tensor)
                 rng.mark_usage(sg_time)
 
     lr_graph.current_time += 1
     return lr_graph
 
 
-def _extract_live_ranges_from_schedule(sg, target_mem_area, target_mem_type_set, lr_graph):
+def extract_live_ranges_from_schedule(sg, target_mem_area, target_mem_type_set, lr_graph, verbose_progress=False):
     time_for_cascade = {}
-    for sched_op in sg.sched_ops:
+    for index, sched_op in enumerate(sg.sched_ops):
+        progress_print(verbose_progress, "Processing SchedulerOp", index, sg.sched_ops)
         op_info = sg.schedule.cost_map[sched_op]
         cascade = op_info.cascade
         cascade_info = sg.schedule.cascades.get(cascade, None)
 
         if cascade_info is None:
             # Op is not part of a cascade, check if the ifm can be overwritten by the ofm
             merge_elementwise_op_ranges(sg, sched_op, lr_graph, target_mem_area, target_mem_type_set)
@@ -374,16 +382,15 @@
 
         if time_to_set == lr_graph.current_time:
             lr_graph.current_time += 2
 
         if cascade != 0:
             time_for_cascade[cascade] = time_to_set
 
-    end_time = lr_graph.update_endtime()
-
+    time_to_set = lr_graph.current_time
     for tens in sg.output_tensors:
         if tens.mem_type not in target_mem_type_set or tens.mem_area != target_mem_area:
             continue
         rng = lr_graph.get_or_create_range(tens)
-        rng.mark_usage(end_time)
+        rng.mark_usage(time_to_set)
 
     return lr_graph
```

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/mark_tensors.py` & `ethos-u-vela-3.8.0/ethosu/vela/mark_tensors.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,18 @@
             continue
         if tens.purpose != TensorPurpose.Unknown:
             purpose = tens.purpose
         elif tens in weight_tensors:
             purpose = TensorPurpose.Weights
         else:
             purpose = TensorPurpose.FeatureMap
+        # Treat Dynamic Weights as FeatureMap to avoid issues during scheduling caused by
+        # having non constant OPs that produce tensors used as weights.
+        if any(op.type != Op.Const and tens == op.ofm and purpose == TensorPurpose.Weights for op in tens.ops):
+            purpose = TensorPurpose.FeatureMap
         mark_purpose(tens, arch, purpose)
     if op.type in memory_only_ops:
         # Memory only operator input and output point to same data
         op.ofm.mem_area = op.ifm.mem_area
 
     if op.type == Op.Custom and op.attrs.get("custom_type") == CustomType.ExistingNpuOp:
         scratch_tensor = None
```

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/model_reader.py` & `ethos-u-vela-3.8.0/ethosu/vela/model_reader.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/nn_graph.py` & `ethos-u-vela-3.8.0/ethosu/vela/nn_graph.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/npu_performance.py` & `ethos-u-vela-3.8.0/ethosu/vela/npu_performance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright 2020-2022 Arm Limited and/or its affiliates <open-source-office@arm.com>
+# SPDX-FileCopyrightText: Copyright 2020-2023 Arm Limited and/or its affiliates <open-source-office@arm.com>
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 # Licensed under the Apache License, Version 2.0 (the License); you may
 # not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -468,14 +468,18 @@
     elif query.npu_block_type == NpuBlockType.ElementWise:
         cycles.op_macs = 0
         ofm_rounding = Shape4D(list(arch.storage_rounding_quantums[query.ofm_format]))
         cycles.op_cycles = round_up_to_int(
             _estimate_output_cycles_per_element(arch, op_type, faf_type, query)
             * Shape4D.round_up(query.ofm_shape, ofm_rounding).elements()
         )
+    # DMA cycle calculation
+    elif query.npu_block_type == NpuBlockType.Dma:
+        # Return 0 since this is not an actual NPU op
+        cycles.op_cycles = 0
     else:
         assert False
 
     return cycles
 
 
 def measure_element_access(arch, query: PerformanceQuery):
@@ -537,14 +541,18 @@
             access.ifm_read[0] = Shape4D.round_up(query.ofm_shape, ifm_rounding).elements()
             if query.ifm2_shape:
                 if query.ifm2_shape.elements() > 1:
                     access.ifm_read[1] = Shape4D.round_up(query.ofm_shape, ifm_rounding).elements()
                 elif query.ifm2_bits > 8:
                     # ifm2 is a non 8-bit scalar
                     access.ifm_read[1] = Shape4D.round_up(query.ifm2_shape, ifm_rounding).elements()
+    # DMA
+    elif query.npu_block_type == NpuBlockType.Dma:
+        # Return empty access since this is not an actual NPU op
+        return access
     # Unknown
     else:
         assert False
 
     ofm_rounding = Shape4D(list(arch.storage_rounding_quantums[query.ofm_format]))
     access.ofm_write = Shape4D.round_up(query.ofm_shape, ofm_rounding).elements()
     return access
@@ -642,26 +650,36 @@
 
     # How many NPU cycles are available under the previously executing
     # operator for performing buffered DMA transfers
     slack_cycles = prev_cost.slack_buffering_cycles if prev_cost else 0
 
     # LUT Transfer
     parent_op = op.parent_op
-    lut_transfer_cycles = 0
+    dma_transfer_cycles = 0
     if parent_op.activation_lut:
         lut_tensor = [tens for tens in parent_op.inputs if tens.purpose == TensorPurpose.LUT][0]
         src_tensor = lut_tensor.src_tensor
         if src_tensor and lut_tensor.mem_area != src_tensor.mem_area:
             bw = src_tensor.storage_size()
-            lut_transfer_cycles = measure_mem2mem_cycles(arch, src_tensor.mem_area, lut_tensor.mem_area, bw)
+            dma_transfer_cycles += measure_mem2mem_cycles(arch, src_tensor.mem_area, lut_tensor.mem_area, bw)
 
             bws[src_tensor.mem_area][lut_tensor.purpose][BandwidthDirection.Read] += bw
             # LUT read from SHRAM TODO remove?
             scaled_bws[lut_tensor.mem_area][lut_tensor.purpose][BandwidthDirection.Read] += bw
 
+    # DMA Transfer
+    if parent_op.type == Op.Memcpy:
+        src_tensor = parent_op.ifm
+        dst_tensor = parent_op.ofm
+        if src_tensor.mem_area != dst_tensor.mem_area:
+            bw = src_tensor.storage_size()
+            dma_transfer_cycles += measure_mem2mem_cycles(arch, src_tensor.mem_area, dst_tensor.mem_area, bw)
+            bws[src_tensor.mem_area][src_tensor.purpose][BandwidthDirection.Read] += bw
+            bws[dst_tensor.mem_area][src_tensor.purpose][BandwidthDirection.Write] += bw
+
     if cost.npu_weights_tensor and cost.buffered_weight_tensors:
         # DMA Weight Transfer
         sz = 0
         # Get the size of the first DMA
         for core in range(0, arch.ncores):
             key = WeightKey(core, 0)
             if key in cost.npu_weights_tensor.encoded_ranges:
@@ -686,19 +704,19 @@
         else:
             # Standard buffer - weights can not be fetched in parallel so weight transfer
             # must be included in the result
             cycles_a[PassCycles.Npu] = (
                 cycles.op_cycles + cost.full_weight_transfer_cycles - min(ws_first_transfer_cycles, slack_cycles)
             )
 
-        # Add cycles for LUT Transfer
-        cycles_a[PassCycles.Npu] += lut_transfer_cycles
+        # Add cycles for LUT + mempcy op Transfer
+        cycles_a[PassCycles.Npu] += dma_transfer_cycles
     else:
-        # Add cycles for LUT Transfer
-        cycles_a[PassCycles.Npu] += max(lut_transfer_cycles - slack_cycles, 0)
+        # Add cycles for LUT + mempcy op Transfer
+        cycles_a[PassCycles.Npu] += max(dma_transfer_cycles - slack_cycles, 0)
 
     # OFM write
     ofm = op.parent_op.ofm
     bw = access.ofm_write * ofm.element_size()
     bws[query.ofm_memory_area][ofm.purpose][BandwidthDirection.Write] += bw
     scaled_bws[ofm.mem_area][ofm.purpose][BandwidthDirection.Write] += _estimate_memory_transfer_efficiency(
         arch, False, query.ofm_memory_area, ofm.format, query.ofm_bits, query.config.ofm_block, query.ofm_shape, bw
@@ -866,15 +884,14 @@
                     w = str(width)
                 else:
                     w = str(width + precision) + "f"
                 line += f"{item:{align}{w}}" + " "
             print(line)
 
         # print to csv
-        writer.writerow((sg_seperator_text,))
         writer.writerow(col_name for col_name, _, _, _ in header)
         for op_data in data:
             writer.writerow(op_data)
 
     # close the csv
     csv_file.close()
```

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/npu_serialisation.py` & `ethos-u-vela-3.8.0/ethosu/vela/npu_serialisation.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/numeric_util.py` & `ethos-u-vela-3.8.0/ethosu/vela/numeric_util.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/operation.py` & `ethos-u-vela-3.8.0/ethosu/vela/operation.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,44 +17,53 @@
 # Description:
 # Internal representation of a Neural Network Operation.
 # For Class name forward references for the type annotations. (see PEP 563).
 from __future__ import annotations
 
 import copy
 from collections import namedtuple
+from enum import auto
 from enum import Enum
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import TYPE_CHECKING
 
-from .api import NpuRoundingMode
 from .errors import VelaError
 from .ethos_u55_regs.ethos_u55_regs import resampling_mode
 from .numeric_util import full_shape
 from .shape4d import Shape4D
 
 # Import needed for Type annotations. Only import for Type checking to avoid run-time errors due to cyclic import.
 if TYPE_CHECKING:
+    from .tensor import QuantizationParameters
     from .tensor import Tensor
 
 PointXY = namedtuple("PointXY", "x y")
 PointXYZ = namedtuple("PointXYZ", "x y z")
 
 
+class RoundingMode(Enum):
+    TFLite = auto()  # Round like TensorFlow Lite
+    ToZero = auto()  # Round towards zero (truncate)
+    HalfUp = auto()  # Round to nearest with x.5 rounded up towards positive infinity (natural)
+    AwayZero = auto()  # Round away from zero (towards infinity)
+
+
 class NpuBlockType(Enum):
     Default = 0
     ConvolutionMxN = 1
     VectorProduct = 2
     Pooling = 3
     ConvolutionDepthWise = 4
     ElementWise = 5
     ReduceSum = 6
+    Dma = 7
 
 
 class Kernel:
     """
     Kernel information for NPU operations
     """
 
@@ -129,24 +138,22 @@
 
 # Internally used operation codes
 class Op(Enum):
     Abs = OperatorInfo(block_type=NpuBlockType.ElementWise, indices=NNG_IFM_INDICES, is_unary=True)
     Add = OperatorInfo(block_type=NpuBlockType.ElementWise, indices=NNG_IFM_IFM2_INDICES)
     AddN = OperatorInfo()
     Any = OperatorInfo()
-    ArgMax = OperatorInfo()
+    ArgMax = OperatorInfo(indices=NNG_IFM_INDICES)
     ArgMin = OperatorInfo()
     AvgPool = OperatorInfo(block_type=NpuBlockType.Pooling, indices=NNG_IFM_INDICES)
     Atan2 = OperatorInfo(indices=NNG_IFM_IFM2_INDICES)
     BatchMatMul = OperatorInfo()
     BatchToSpaceND = OperatorInfo()
     BidirectionalSequenceLstm = OperatorInfo(block_type=NpuBlockType.VectorProduct, indices=NNG_IFM_WEIGHTS_INDICES)
     BidirectionalSequenceRnn = OperatorInfo(block_type=NpuBlockType.VectorProduct, indices=NNG_IFM_WEIGHTS_INDICES)
-    BlockLSTM = OperatorInfo(block_type=NpuBlockType.VectorProduct, indices=NNG_BLOCK_LSTM_INDICES)
-
     CLZ = OperatorInfo(
         block_type=NpuBlockType.ElementWise, indices=NNG_IFM_INDICES, is_unary=True
     )  # NPU specific operation
     Call = OperatorInfo()
     Cast = OperatorInfo()
     Ceil = OperatorInfo()
     Clamp = OperatorInfo(indices=NNG_IFM_INDICES)  # TOSA specific
@@ -170,19 +177,20 @@
     Densify = OperatorInfo()
     DepthToSpace = OperatorInfo()
     DepthwiseConv2DBias = OperatorInfo(
         block_type=NpuBlockType.ConvolutionDepthWise, indices=NNG_IFM_WEIGHTS_BIAS_INDICES
     )
     Dequantize = OperatorInfo(indices=NNG_IFM_INDICES)
     Div = OperatorInfo()
+    Memcpy = OperatorInfo(block_type=NpuBlockType.Dma, indices=NNG_IFM_INDICES)
     Elu = OperatorInfo()
     EmbeddingLookup = OperatorInfo()
     EmbeddingLookupSparse = OperatorInfo()
     Equal = OperatorInfo()
-    Exp = OperatorInfo()
+    Exp = OperatorInfo(block_type=NpuBlockType.ElementWise, indices=NNG_IFM_INDICES, is_unary=True)
     ExpandDims = OperatorInfo(indices=NNG_IFM_INDICES)
     FakeQuantWithMinMaxArgs = OperatorInfo()
     Fill = OperatorInfo()
     Floor = OperatorInfo()
     FloorDiv = OperatorInfo()
     FloorMod = OperatorInfo()
     FullyConnected = OperatorInfo(block_type=NpuBlockType.VectorProduct, indices=NNG_IFM_WEIGHTS_BIAS_INDICES)
@@ -291,14 +299,15 @@
     TopKV2 = OperatorInfo()
     Transpose = OperatorInfo(indices=NNG_IFM_IFM2_INDICES)
     UnidirectionalSequenceLstm = OperatorInfo(block_type=NpuBlockType.VectorProduct, indices=NNG_IFM_WEIGHTS_INDICES)
     UnidirectionalSequenceRnn = OperatorInfo(block_type=NpuBlockType.VectorProduct, indices=NNG_IFM_WEIGHTS_INDICES)
     Unique = OperatorInfo()
     Unpack = OperatorInfo(indices=NNG_IFM_INDICES)
     UnpackReshaped = OperatorInfo(indices=NNG_IFM_INDICES)
+    VariableTensorWrite = OperatorInfo()
     Where = OperatorInfo()
     While = OperatorInfo()
     ZerosLike = OperatorInfo()
     CallOnce = OperatorInfo()
     BroadcastTo = OperatorInfo()
     Rfft2D = OperatorInfo()
     Conv3D = OperatorInfo()
@@ -369,14 +378,17 @@
 
     def is_concat_op(self):
         return self in (Op.Concat, Op.ConcatTFLite, Op.PackReshaped, Op.Pack)
 
     def is_resize_op(self):
         return self in (Op.ResizeBilinear, Op.ResizeNearestNeighbor)
 
+    def is_memcpy_op(self):
+        return self.info.block_type == NpuBlockType.Dma
+
     def needs_bias(self):
         return bool(self.info.indices.biases)
 
     def needs_shapes(self):
         return bool(self.info.indices.ifms)
 
     @classmethod
@@ -462,14 +474,15 @@
     """Class representing a Neural Network operation. Has a name, a type,
     input and output tensors, as well as an attribute dictionary."""
 
     __slots__ = (
         "type",
         "_original_type",
         "name",
+        "version",
         "op_index",
         "attrs",
         "inputs",
         "outputs",
         "intermediates",
         "flops",
         "scheduled_pass",
@@ -481,57 +494,54 @@
         "activation_lut",
         "_kernel",
         "ifm_shapes",
         "ofm_shapes",
         "rescale",
         "read_offsets",
         "read_shapes",
-        "rounding_mode",
+        "_rounding_mode",
         "explicit_scaling",
-        "low_precision_scaling",
         "write_offset",
         "write_shape",
         "ifm_resampling_mode",
         "tile_base_offsets_ifm",
         "tile_base_offsets_ofm",
         "ofm_stride_multiplier",
     )
 
     def __init__(self, op_type: Op, name: str):
         self.type = op_type
         self._original_type = op_type  # the original type of the operation. once set this shouldn't be changed
         self.name = name
+        self.version = 1  # Used to track original operator version.
         self.attrs: Dict[str, Any] = {}
         self.inputs: List[Optional[Tensor]] = []
         self.outputs: List[Tensor] = []
         self.intermediates: List[Tensor] = []
         self.flops = 0
         self.run_on_npu = True
         # Fused activation function. If not none: operator code.
         self.activation: Optional[ActivationFunction] = None
         # Fused memory function, if not None: operator code
         self.memory_function: Optional[Op] = None
         # If not none: contains QuantizationParameters to be used as output quantization
         # (which overrides the ofm tensor's quantization), used in LUT
-        self.forced_input_quantization = None
-        self.forced_output_quantization = None
+        self.forced_input_quantization: Optional[QuantizationParameters] = None
+        self.forced_output_quantization: Optional[QuantizationParameters] = None
         self.scheduled_pass = None
         self.op_index = None  # input network operator index
         self.activation_lut = None
         self._kernel = None
         self.ifm_shapes: List[Shape4D] = []
         self.ofm_shapes: List[Shape4D] = []
         self.read_offsets: List[Optional[Shape4D]] = [None, None]  # offset for [ifm, ifm2]
         self.read_shapes: List[Optional[Shape4D]] = [None, None]  # read shape for [ifm, ifm2]
-        self.rounding_mode: Optional[NpuRoundingMode] = None
+        self._rounding_mode: Optional[RoundingMode] = None
         # Rescale op in TOSA supplies explicit multiplier and shift values
         self.explicit_scaling: Optional[ExplicitScaling] = None
-        # The Mean operator (implemented as a depthwise convolution) requires scaling
-        # to be calculated differently in one case. In that case, this is set to True.
-        self.low_precision_scaling = False
         # Write offset, for operations that only produce a part of the OFM
         self.write_offset: Optional[Shape4D] = None
         # The amount of OFM that is produced by the operation (only if write_offset is not None).
         # E.g. an operation that only fills the bottom row of an OFM of size 1x10x8x1 would have
         # write_offset 0,9,0,0, write_shape 1,1,8,1
         self.write_shape: Optional[Shape4D] = None
         self.ifm_resampling_mode: resampling_mode = resampling_mode.NONE
@@ -544,15 +554,15 @@
         self.ofm_stride_multiplier: List[int] = [1, 1, 1]
 
     def clone(self, suffix="_clone"):
         res = Operation(self.type, self.name + suffix)
 
         # maintain the original type, in cases where the type was changed to something different
         res._original_type = self._original_type
-
+        res.version = self.version
         res.attrs = dict(self.attrs)
         res.inputs = list(self.inputs)
         res.outputs = list(self.outputs)
         res.intermediates = list(self.intermediates)
         res.flops = self.flops
         res.run_on_npu = self.run_on_npu
         res.activation = None if self.activation is None else self.activation.clone()
@@ -563,15 +573,14 @@
         res.op_index = None  # not relevant as not part of input network
         res.read_offsets = list(self.read_offsets)
         res.read_shapes = list(self.read_shapes)
         res.write_offset = Shape4D(*self.write_offset) if self.write_offset else None
         res.write_shape = Shape4D(*self.write_shape) if self.write_shape else None
         res.rounding_mode = self.rounding_mode
         res.explicit_scaling = self.explicit_scaling
-        res.low_precision_scaling = self.low_precision_scaling
         res.ifm_resampling_mode = self.ifm_resampling_mode
         res.tile_base_offsets_ifm = [_ifm.copy() for _ifm in self.tile_base_offsets_ifm]
         res.tile_base_offsets_ofm = self.tile_base_offsets_ofm.copy()
         res.ofm_stride_multiplier = self.ofm_stride_multiplier.copy()
 
         return res
 
@@ -581,14 +590,46 @@
     __repr__ = __str__
 
     @property
     def original_type(self):
         return self._original_type
 
     @property
+    def rounding_mode(self):
+        return self._rounding_mode
+
+    @rounding_mode.setter
+    def rounding_mode(self, mode: RoundingMode):
+        # All rounding modes are supported by all operators with the exception of rounding away from zero (see comment
+        # below)
+        is_supported = True
+        if mode == RoundingMode.AwayZero:
+            # Rounding away from zero does not have direct hardware support and so the compiler implements it indirectly
+            # in different ways. The exact process depends upon the operator type and not all operators are supported.
+            # Basically, rounding away from zero works by adjusting the accumulated value by a "small" amount before
+            # rounding up with the addition of a half (natural rounding). This "small" amount should be big enough to
+            # cause x.5 to be rounded correctly but small enough that smaller values are not incorrectly rounded. This
+            # is done by slightly adjusting the scale and shift on the ofm tensor using the scale and bias tensor,
+            # it has no affect on global scaling (i.e. the ofm_scale register). In addition, the zero points of the
+            # input and/or output tensors may also require forcing to zero but the exact behaviour also depends upon the
+            # corresponding optimisation performed in graph_optimisation.py where the rounding mode is set
+            is_supported = False
+            if self.original_type == Op.ResizeBilinear and self.type == Op.DepthwiseConv2DBias:
+                is_supported = True
+            if self.original_type == Op.AvgPool and self.type == Op.DepthwiseConv2DBias:
+                is_supported = True
+
+        if is_supported:
+            self._rounding_mode = mode
+        else:
+            assert (
+                False
+            ), f"Setting rounding mode = {mode} on {self.original_type} operator '{self.name}' is not supported."
+
+    @property
     def type_changed(self):
         return self.type != self.original_type
 
     def get_kernel_size(self):
         weights = self.weights
         if weights and self.type.npu_block_type in (NpuBlockType.ConvolutionDepthWise, NpuBlockType.ConvolutionMxN):
             weight_shape = full_shape(4, weights.shape, 1)
@@ -850,23 +891,14 @@
 
     def set_ifm_ofm_shapes(self):
         self.ifm_shapes = []
         self.ofm_shapes = []
 
         ifm_tensor, ifm2_tensor, ofm_tensor = self.get_ifm_ifm2_ofm()
 
-        if self.type == Op.Reshape:
-            # Set ofm shape
-            if len(self.inputs) > 1 and self.inputs[1].values is not None:
-                ofm_tensor.shape = self.inputs[1].values.flatten().tolist()
-                ofm_elements = ofm_tensor.elements()
-                # Stretch dimension
-                if ofm_elements < 0:
-                    ofm_tensor.shape[ofm_tensor.shape.index(-1)] = int(ifm_tensor.elements() / abs(ofm_elements))
-
         # set all shapes to op, as 4D
         if self.type == Op.FullyConnected:
             if len(self.ifm.shape) == 2:
                 self.ifm_shapes.append(Shape4D([self.ifm.shape[0], 1, 1, self.ifm.shape[1]]))
             else:
                 # Special case, handled in graph optimization
                 self.ifm_shapes.append(Shape4D(ifm_tensor.get_full_shape()))
```

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/operation_util.py` & `ethos-u-vela-3.8.0/ethosu/vela/operation_util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright 2020-2022 Arm Limited and/or its affiliates <open-source-office@arm.com>
+# SPDX-FileCopyrightText: Copyright 2020-2023 Arm Limited and/or its affiliates <open-source-office@arm.com>
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 # Licensed under the Apache License, Version 2.0 (the License); you may
 # not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -15,21 +15,26 @@
 # limitations under the License.
 #
 # Description:
 # Utility functions for creating Network Operations.
 from typing import Optional
 from typing import Tuple
 
+import numpy as np
+
 from .data_type import DataType
 from .high_level_command_to_npu_op import ifm_ifm2_correct_order
 from .operation import ActivationFunction
 from .operation import Op
 from .operation import Operation
 from .operation import Padding
+from .reader_util import clone_and_reshape_tensor
 from .shape4d import Shape4D
+from .tensor import create_const_tensor
+from .tensor import create_equivalence_id
 from .tensor import QuantizationParameters
 from .tensor import Tensor
 
 
 def create_avgpool_nop(name: str) -> Operation:
     op = Operation(Op.AvgPool, name)
     op.attrs["padding"] = Padding.VALID
@@ -47,20 +52,126 @@
 
 def create_add_nop(name: str) -> Operation:
     op = Operation(Op.Add, name)
     op.run_on_npu = True
     return op
 
 
+def create_memcpy(
+    name: str,
+    ifm: Tensor,
+    ofm: Tensor,
+) -> Operation:
+    op = Operation(Op.Memcpy, name)
+    op.run_on_npu = True
+    op.add_input_tensor(ifm)
+    op.set_output_tensor(ofm)
+    op.set_ifm_ofm_shapes()
+    return op
+
+
 def create_pad_nop(name: str) -> Operation:
     op = Operation(Op.Pad, name)
     op.run_on_npu = True
     return op
 
 
+def create_cast_op(
+    name: str,
+    ifm: Tensor,
+    ofm: Tensor,
+) -> Operation:
+    op = Operation(Op.DepthwiseConv2DBias, name)
+    op_attrs = {
+        "padding": Padding.VALID,
+        "stride_h": 1,
+        "stride_w": 1,
+        "strides": (1, 1, 1, 1),
+        "depth_multiplier": 1,
+        "channel_multiplier": 1,
+        "dilation_h_factor": 1,
+        "dilation_w_factor": 1,
+        "dilation": (1, 1, 1, 1),
+        "explicit_padding": None,
+    }
+    op.attrs.update(op_attrs)
+    op.add_input_tensor(ifm)
+
+    c = ifm.shape[-1]
+
+    shape = [1, 1, 1, c]
+    kernel = np.dstack([1] * c)
+    identity_quant = QuantizationParameters(scale_f32=1.0, zero_point=0)
+    op.add_input_tensor(
+        create_const_tensor(
+            op.name + "_weights",
+            shape,
+            DataType.uint8,
+            np.array(kernel).reshape(shape),
+            quantization=identity_quant,
+        ),
+    )
+    bias_values = [0] * c
+    dtype = DataType.int64 if op.ifm.dtype == DataType.int16 else DataType.int32
+    op.add_input_tensor(create_const_tensor(op.name + "_bias", [c], dtype, bias_values))
+    op.set_output_tensor(ofm)
+    op.set_ifm_ofm_shapes()
+
+    return op
+
+
+def create_fused_activation(op_type: Op, name: str, ifm: Tensor, quantization: QuantizationParameters) -> Operation:
+    assert op_type.is_activation_op()
+    op = create_avgpool_nop(name)
+    op.activation = ActivationFunction(op_type)
+    ofm = Tensor(ifm.shape, ifm.dtype, f"{op.name}_tens0")
+    ofm.quantization = quantization
+    op.add_input_tensor(ifm)
+    op.set_output_tensor(ofm)
+    op.set_ifm_ofm_shapes()
+    return op
+
+
+def create_fullyconnected(
+    name: str,
+    ifm: Tensor,
+    weights: Tensor,
+    bias: Optional[Tensor],
+    quantization: QuantizationParameters,
+    vela_weight_order: bool = True,
+) -> Operation:
+    # Reshape weights if needed
+    if not vela_weight_order:
+        weights = clone_and_reshape_tensor(weights, (1, 0), False)
+
+    n_ofm = weights.shape[-1]
+
+    # Setup bias if needed
+    if not bias:
+        bias_values = [0] * n_ofm
+        dtype = DataType.int64 if ifm.dtype == DataType.int16 else DataType.int32
+        bias = create_const_tensor(f"{name}_bias", [n_ofm], dtype, bias_values)
+        # Set equivalence_id based on values to avoid placing duplicate data in flash
+        bias.equivalence_id = create_equivalence_id(tuple(bias_values))
+        bias.value_id = bias.equivalence_id
+
+    # Setup ofm
+    ofm = Tensor([ifm.shape[0], n_ofm], ifm.dtype, f"{name}_tens0")
+    ofm.quantization = quantization
+
+    # Create op and add tensors
+    op = Operation(Op.FullyConnected, name)
+    op.add_input_tensor(ifm)
+    op.add_input_tensor(weights)
+    op.add_input_tensor(bias)
+    op.set_output_tensor(ofm)
+    op.set_ifm_ofm_shapes()
+    return op
+
+
 def create_depthwise_maxpool(
     name: str,
     ifm: Tensor,
     inp_shape: Shape4D,
     quantization: QuantizationParameters,
     activation: Optional[ActivationFunction] = None,
 ) -> Operation:
```

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/pass_packing.py` & `ethos-u-vela-3.8.0/ethosu/vela/pass_packing.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     Mac = 4
     ElementWise = 8
     Npu = 16
     Cpu = 32
     StartupInit = 64
     MemoryOnly = 128
     PostFusingLimited = 256
+    Memcpy = 512
 
 
 mac_main_ops = set(
     (
         # convolutions
         Op.Conv2DBias,
         Op.Conv2D,
@@ -50,16 +51,14 @@
         Op.Conv2DBackpropInputSwitchedBias,
         # depth-wise convolutions
         Op.DepthwiseConv2DBias,
         # FC layers
         Op.QuantizedMatMul,
         Op.MatMul,
         Op.FullyConnected,
-        # RNN/LSTM/GRU
-        Op.BlockLSTM,
         # pooling
         Op.QuantizedMaxPool,
         Op.QuantizedAvgPool,
         Op.AvgPool,
         Op.MaxPool,
         Op.ReduceSum,
     )
@@ -91,14 +90,15 @@
     (
         Op.Squeeze,
         Op.Reshape,
         Op.QuantizedReshape,
         Op.ExpandDims,
     )
 )
+memcpy_ops = set((Op.Memcpy,))
 
 
 test_sequence = [
     (
         # ops_set
         npu_post_ops,
         # incompatible_pack_flags
@@ -156,14 +156,24 @@
         # flags_to_set
         PassFlags.MemoryOnly | PassFlags.Main,
         # flags_to_clear
         PassFlags.Empty,
     ),
     (
         # ops_set
+        memcpy_ops,
+        # incompatible_pack_flags
+        PassFlags.Cpu | PassFlags.MemoryOnly | PassFlags.Mac | PassFlags.Main | PassFlags.PostFusingLimited,
+        # flags_to_set
+        PassFlags.Npu | PassFlags.Memcpy | PassFlags.Main,
+        # flags_to_clear
+        PassFlags.Empty,
+    ),
+    (
+        # ops_set
         cpu_ops,
         # incompatible_pack_flags
         PassFlags.Npu | PassFlags.MemoryOnly | PassFlags.Main,
         # flags_to_set
         PassFlags.Cpu | PassFlags.Main,
         # flags_to_clear
         PassFlags.Empty,
@@ -244,15 +254,19 @@
                             primary_op = curr_op
 
                         curr_flags &= ~flags_to_clear
                         curr_flags |= flags_to_set
 
                         if flags_to_set & PassFlags.Npu:
                             if flags_to_set & (
-                                PassFlags.Mac | PassFlags.ElementWise | PassFlags.Post | PassFlags.PostFusingLimited
+                                PassFlags.Mac
+                                | PassFlags.ElementWise
+                                | PassFlags.Post
+                                | PassFlags.PostFusingLimited
+                                | PassFlags.Memcpy
                             ):
                                 assert len(curr_op.inputs) >= 1
                                 ifm_tensor = curr_op.ifm
                                 ifm_shapes = curr_op.ifm_shapes.copy()
                                 assert ifm_tensor is not None, "IFM missing in {}".format(curr_op)
                                 assert ifm_tensor.purpose == TensorPurpose.FeatureMap
 
@@ -516,19 +530,20 @@
                 if next_ps.placement == PassPlacement.Cpu:
                     # It is possible to move the CPU pass
                     pass_list.remove(cpu_ps)
                     insert_index = pass_list.index(next_ps)
                     pass_list.insert(insert_index, cpu_ps)
                     break
 
+                # Check all outputs from the cpu pass
                 if (
-                    cpu_ps.ops[0].ofm in [next_ps.ops[0].ifm, next_ps.ops[0].ifm2]
+                    any(ofm in [next_ps.ops[0].ifm, next_ps.ops[0].ifm2] for ofm in cpu_ps.ops[0].outputs)
                     or next_ps.placement == PassPlacement.MemoryOnly
                 ):
-                    # Not possible to move
+                    # Not possible to move since next pass depends on the output from the cpu pass
                     break
 
                 if pass_list.index(next_ps) == last_idx:
                     # Last element, ok to move the CPU pass
                     pass_list.remove(cpu_ps)
                     pass_list.append(cpu_ps)
                     break
```

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/range_set.py` & `ethos-u-vela-3.8.0/ethosu/vela/range_set.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/rawdata_writer.py` & `ethos-u-vela-3.8.0/ethosu/vela/rawdata_writer.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/reader_util.py` & `ethos-u-vela-3.8.0/ethosu/vela/reader_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     for tens in input_tensors:
         if len(tens.ops) and tens.ops[0].type == Op.Const:
             break
 
         if tens.ops != []:
             tens.error("This subgraph input tensor has unexpected driving operators.")
 
-        op = Operation(Op.Placeholder, tens.name)
+        op = Operation(Op.Placeholder if tens.values is None else Op.Const, tens.name)
         op.set_output_tensor(tens)
 
     for tens in tensors:
         if not tens.ops:
             op = Operation(Op.Placeholder if tens.is_variable else Op.Const, tens.name)
             op.set_output_tensor(tens)
```

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/register_command_stream_generator.py` & `ethos-u-vela-3.8.0/ethosu/vela/register_command_stream_generator.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/register_command_stream_util.py` & `ethos-u-vela-3.8.0/ethosu/vela/register_command_stream_util.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/rewrite_graph.py` & `ethos-u-vela-3.8.0/ethosu/vela/rewrite_graph.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/scaling.py` & `ethos-u-vela-3.8.0/ethosu/vela/scaling.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/scheduler.py` & `ethos-u-vela-3.8.0/ethosu/vela/scheduler.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import TYPE_CHECKING
 
+from .utils import progress_print
+
 # Import needed for Type annotations. Only import for Type checking to avoid run-time errors due to cyclic import.
 if TYPE_CHECKING:
     from .npu_performance import CycleCost
 
 import numpy as np
 
 from . import live_range
@@ -56,15 +58,14 @@
 from .nn_graph import Pass
 from .nn_graph import PassPlacement
 from .nn_graph import SchedulingStrategy
 from .nn_graph import Subgraph
 from .live_range import ofm_can_reuse_ifm
 from .numeric_util import round_down
 from .numeric_util import round_up
-from .operation import NpuBlockType
 from .operation import Op
 from .shape4d import Shape4D
 from .tensor import MemArea
 from .tensor import MemType
 from .tensor import Tensor
 from .tensor import TensorFormat
 from .tensor import TensorPurpose
@@ -145,18 +146,20 @@
     """Contains options for the Scheduler"""
 
     def __init__(
         self,
         optimization_strategy,
         sram_target,
         verbose_schedule,
+        verbose_progress=False,
     ):
         self.optimization_strategy = optimization_strategy
         self.optimization_sram_limit = sram_target
         self.verbose_schedule = verbose_schedule
+        self.verbose_progress = verbose_progress
 
     def __str__(self) -> str:
         return f"{type(self).__name__}: {str(self.__dict__)}"
 
     __repr__ = __str__
 
 
@@ -209,14 +212,22 @@
         self.ofm = SchedulerTensor(
             ps.ofm_shapes[0],
             ps.ofm_tensor.dtype,
             ps.ofm_tensor.mem_area,
             ps.ofm_tensor.format,
         )
 
+        # LUT must be placed in shram area. The copy is done by DMA
+        # generated by the high level command stream generator.
+        for idx, tens in enumerate(self.parent_op.inputs):
+            if tens.purpose == TensorPurpose.LUT:
+                new_tens = tens.clone_into_shram(self.arch)
+                new_tens.consumer_list.append(self.parent_op)
+                self.parent_op.inputs[idx] = new_tens
+
         # Input volume width and height required to produce the smallest possible stripe
         self.min_stripe_input_w, self.min_stripe_input_h = self._calculate_min_stripe_input()
 
         # Flags that marks whether this SchedulerOperation requires full IFM/OFM
         self.requires_full_ifm = False
         self.requires_full_ifm2 = False
         self.requires_full_ofm = False
@@ -456,19 +467,19 @@
         for ps in self.sg.passes:
             if ps.primary_op:
                 # Set tensor format to NHCWB16 for output FeatureMaps, if possible
                 for output in ps.outputs:
                     if output in self.sg.output_tensors or output.purpose != TensorPurpose.FeatureMap:
                         continue
 
-                    if output.needs_linear_format:
+                    if output.use_linear_format:
                         continue
 
                     if self.avoid_nhcwb16_for_ofm(output, ps, arch):
-                        output.needs_linear_format = True
+                        output.force_linear_format = True
                         continue
 
                     output.set_format(TensorFormat.NHCWB16, arch)
 
                 # Create SchedulerOperations
                 op = SchedulerOperation(ps, arch, self.nng)
                 op.index = len(self.sched_ops)
@@ -493,19 +504,19 @@
                     op.requires_full_ifm = True
                 if ps.ifm2_tensor and ps.ifm2_tensor in self.sg.input_tensors:
                     # This Op consumes a subgraph input
                     op.requires_full_ifm2 = True
                 if ps.ofm_tensor in self.sg.output_tensors:
                     # This Op produces a subgraph output
                     op.requires_full_ofm = True
-                if ps.ifm_tensor.needs_linear_format:
+                if ps.ifm_tensor.use_linear_format:
                     op.requires_full_ifm = True
-                if ps.ifm2_tensor and ps.ifm2_tensor.needs_linear_format:
+                if ps.ifm2_tensor and ps.ifm2_tensor.use_linear_format:
                     op.requires_full_ifm2 = True
-                if ps.ofm_tensor.needs_linear_format or ps.primary_op.memory_function == Op.ConcatSliceWrite:
+                if ps.ofm_tensor.use_linear_format or ps.primary_op.memory_function == Op.ConcatSliceWrite:
                     op.requires_full_ofm = True
                 if len(ps.primary_op.outputs) > 1 or len(ps.primary_op.outputs[0].consumer_list) > 1:
                     # Op has multiple outputs or consumers - requires full OFM
                     op.requires_full_ofm = True
 
                 # Check memory requirements if this Op requires any full FeatureMaps
                 op_memory_req = 0
@@ -520,34 +531,31 @@
 
         # Theoretical minimum required memory - used to guide the cascade building
         self.min_memory_req = min_memory_req
 
     def create_initial_schedule(self) -> Schedule:
         """Creates an initial schedule with no cascading or buffering of any kind"""
         schedule = Schedule(self.sg, "MAX")
-        for op in self.sched_ops:
+        verbose_progress = self.scheduler_options.verbose_progress
+        for index, op in enumerate(self.sched_ops):
+            progress_print(verbose_progress, "Processing SchedulerOp", index, self.sched_ops)
             cost = op.create_scheduler_info(self.nng, op.ofm.shape)
             cost.cycles = self.estimate_op_performance(op, cost.block_config, op.ofm.shape.depth)
             schedule.cost_map[op] = cost
 
         return schedule
 
     def update_op_memory_snapshot(self, schedule: Schedule):
         memories_list = [(self.arch.fast_storage_mem_area, set((MemType.Scratch, MemType.Scratch_fast)))]
-
+        verbose_progress = self.scheduler_options.verbose_progress
+        progress_print(verbose_progress, "")
         # Collect live ranges from tensors
         lr_graph = live_range.LiveRangeGraph()
         for mem_area, mem_type_set in memories_list:
-            live_range.extract_live_ranges_from_cascaded_passes(
-                self.nng.get_root_subgraph(),
-                mem_area,
-                mem_type_set,
-                lr_graph,
-                Tensor.AllocationQuantum,
-            )
+            live_range.extract_live_ranges_from_schedule(self.sg, mem_area, mem_type_set, lr_graph, verbose_progress)
 
         # Populate time-array with memory used by live ranges
         temporal_usage = lr_graph.get_temporal_memory_usage(self.arch.fast_storage_mem_area)
         schedule.memory_snapshot = temporal_usage
 
         # Set the peak memory usage
         schedule.fast_storage_peak_usage = max(temporal_usage, default=0)
@@ -597,17 +605,18 @@
         query.config = block_config
 
         return npu_performance.measure_element_access(self.arch, query)
 
     def propose_schedule_buffering(self, ref_schedule: Schedule, staging_limit_bytes):
         """Create a buffered schedule"""
         buffered_schedule = Schedule(self.sg, f"{ref_schedule.label}_BUFFERED")
-
+        verbose_progress = self.scheduler_options.verbose_progress
         prev_op = None
-        for sched_op in self.sched_ops:
+        for index, sched_op in enumerate(self.sched_ops):
+            progress_print(verbose_progress, "Processing SchedulerOp", index, self.sched_ops)
             if sched_op not in ref_schedule.cost_map:
                 # sched_op is not part of this sub-schedule - skip
                 continue
 
             self.propose_operator_buffering(sched_op, prev_op, buffered_schedule, ref_schedule, staging_limit_bytes)
             prev_op = sched_op
 
@@ -861,18 +870,19 @@
         return buffered_weight_tensor
 
     def propose_minimal_schedule(self) -> Schedule:
         """Proposes scheduling parameters where every operator is subdivided into the smallest stripe that satisfies the
         next operators stride"""
         min_schedule = Schedule(self.sg, "MIN")
         cost_map = min_schedule.cost_map
-
+        verbose_progress = self.scheduler_options.verbose_progress
         # Keep track of the previous Op - which consumes the current Op's OFM
         prev_op: Optional[SchedulerOperation] = None
-        for sched_op in reversed(self.sched_ops):
+        for index, sched_op in enumerate(reversed(self.sched_ops)):
+            progress_print(verbose_progress, "Processing SchedulerOp", index, self.sched_ops)
             min_stripe_height = prev_op.kernel.stride.y if prev_op else 1
             min_stripe = sched_op.ofm.shape.with_height(min_stripe_height)
 
             cost = sched_op.create_scheduler_info(self.nng, min_stripe)
             cost.cycles = self.estimate_op_performance(sched_op, cost.block_config, sched_op.ofm.shape.depth)
             cost_map[sched_op] = cost
 
@@ -942,38 +952,39 @@
             if sched_op not in cost:
                 # sched_op is not part of the sub-schedule - skip
                 continue
 
             if cost[sched_op].cascade:
                 # This Op is part of a cascade - use the cascade's memory usage
                 cascade_info = cascades[cost[sched_op].cascade]
-                # Non-local memory usage is already included in the cascade_info
-                peak_mem_usage = max(cascade_info.mem_usage, peak_mem_usage)
+                op_mem_usage = cascade_info.mem_usage + non_local_mem_usage.get(sched_op, 0)
             else:
                 # This Op is not part of a cascade - calculate the memory usage
                 op_weight_buffer = sum(tens.storage_size() for tens in cost[sched_op].buffered_weight_tensors)
 
                 op_mem_usage = (
                     sched_op.ifm_size_in_bytes()
                     + sched_op.ofm_size_in_bytes()
                     + op_weight_buffer
                     + non_local_mem_usage.get(sched_op, 0)
                 )
-                peak_mem_usage = max(op_mem_usage, peak_mem_usage)
+            peak_mem_usage = max(op_mem_usage, peak_mem_usage)
 
         return peak_mem_usage
 
     def build_cascades_for_min_schedule(self, min_schedule: Schedule, max_template: Schedule, memory_limit: int):
+        verbose_progress = self.scheduler_options.verbose_progress
         # Update memory snapshot
         self.sg.schedule = min_schedule
         self.update_op_memory_snapshot(min_schedule)
 
         # Calculate residual memory for Min schedule
         non_local_mem_usage = {}
-        for sched_op in self.sched_ops:
+        for index, sched_op in enumerate(self.sched_ops):
+            progress_print(verbose_progress, "Processing SchedulerOp", index, self.sched_ops)
             time_index = min_schedule.cost_map[sched_op].time_index
 
             if self.arch.is_spilling_enabled():
                 # For Dedicated SRAM only the intermediate buffers are in SRAM, hence op_mem_usage is 0
                 op_mem_usage = 0
             else:
                 # Min schedule only have ifm and ofm in SRAM (no buffered weigth tensors)
@@ -1011,17 +1022,19 @@
         # Use the memory snapshot from the reference schedule
         sub_schedule.memory_snapshot = ref_schedule.memory_snapshot
 
         # Calculate memory usage that is live during the sub-schedule but not part of it
         time_for_cascade = ref_cost[sub_schedule_ops[0]].time_index
         mem_usage_parallel_to_sub_schedule = ref_schedule.memory_snapshot[time_for_cascade] - cascade_info.mem_usage
         # If the first Op's IFM has other consumers it has to live throughout the whole sub-schedule whether it's
-        # included in a cascade or not
+        # included in a cascade or not. Not valid in Dedicated SRAM mode (spilling enabled).
         persistent_initial_ifm = (
-            sub_schedule_ops[0].ifm_size_in_bytes() if len(sub_schedule_ops[0].ifm.connection.consumers) > 1 else 0
+            sub_schedule_ops[0].ifm_size_in_bytes()
+            if not self.arch.is_spilling_enabled() and len(sub_schedule_ops[0].ifm.connection.consumers) > 1
+            else 0
         )
         # Calculate non-local-mem-usage per Operator
         non_local_mem_usage = {}
         for idx, sched_op in enumerate(sub_schedule_ops):
             non_local_mem_usage[sched_op] = mem_usage_parallel_to_sub_schedule
             if idx != 0:
                 non_local_mem_usage[sched_op] += persistent_initial_ifm
@@ -1078,21 +1091,24 @@
         self,
         schedule: Schedule,
         max_sched: Schedule,
         max_template: Schedule,
         options: SchedulerOptions,
     ) -> Schedule:
         """Extracts sub-schedules based on the cascades and optimizes them and applies them to the final schedule"""
+        verbose_progress = options.verbose_progress
         sram_limit = options.optimization_sram_limit
         if max_sched.fast_storage_peak_usage < sram_limit and not self.arch.is_spilling_enabled():
             # Maximum performance schedule fits within the SRAM target
             return max_sched
 
         # Iterate over a copy of the cascades since they may change during the loop
-        for cascade_info in list(schedule.cascades.values()):
+        cascades = list(schedule.cascades.values())
+        for index, cascade_info in enumerate(cascades):
+            progress_print(verbose_progress, "Processing cascade", index, cascades)
             # Optimize the sub-schedule in this cascade
             opt_sub_schedule = self.optimize_sub_schedule(cascade_info, schedule, max_template, sram_limit)
             if opt_sub_schedule:
                 # Remove the existing cascade
                 del schedule.cascades[cascade_info.end]
                 # Update the sub-schedule Op and cascade costs to the full schedule
                 schedule.cost_map.update(opt_sub_schedule.cost_map)
@@ -1108,14 +1124,15 @@
         return optimized_sched
 
     def optimize_weight_buffering_size(
         self,
         min_schedule: Schedule,
         options: SchedulerOptions,
     ):
+        verbose_progress = options.verbose_progress
         default_schedule = self.sg.schedule
         npu_performance.calc_new_performance_for_network(self.nng, self.arch, None, False)
         default_tot_cycles = self.nng.cycles[npu_performance.PassCycles.Total]
         default_dram_cycles = self.nng.cycles[npu_performance.PassCycles.DramAccess]
 
         # Restore mem/type for scratched_fms
         for tens in self.scratched_fms:
@@ -1124,21 +1141,15 @@
 
         self.update_op_memory_snapshot(self.sg.schedule)
 
         # Collect live ranges from tensors
         memories_list = [(self.arch.fast_storage_mem_area, set((MemType.Scratch, MemType.Scratch_fast)))]
         lr_graph = live_range.LiveRangeGraph()
         for mem_area, mem_type_set in memories_list:
-            live_range.extract_live_ranges_from_cascaded_passes(
-                self.nng.get_root_subgraph(),
-                mem_area,
-                mem_type_set,
-                lr_graph,
-                Tensor.AllocationQuantum,
-            )
+            live_range.extract_live_ranges_from_schedule(self.sg, mem_area, mem_type_set, lr_graph, verbose_progress)
 
         # Find the relation between the sched_op and the buffering tensor
         weight_ops = {}
         for sched_op in self.sched_ops:
             cost = self.sg.schedule.cost_map[sched_op]
             for tens in cost.buffered_weight_tensors:
                 weight_ops[tens] = sched_op
@@ -1232,33 +1243,37 @@
         self.evicted_fms = []
 
         # Force all OFMs to fast-storage
         for sched_op in self.sched_ops:
             cost = schedule.cost_map[sched_op]
             if cost.cascade == 0 and sched_op.get_dependants():
                 ofm_tens = sched_op.ofm.connection.parent_tens
-                if not any(cons is None for cons in ofm_tens.consumer_list):
+                # Do not move subgraph outputs or Variable Tensor Writes
+                if (
+                    not any(cons is None for cons in ofm_tens.consumer_list)
+                    and sched_op.parent_op.memory_function is not Op.VariableTensorWrite
+                ):
                     if ofm_tens not in self.scratched_fms:
                         # Remember default mem area and mem type, only done once
                         self.scratched_fms[ofm_tens] = (ofm_tens.mem_area, ofm_tens.mem_type)
 
                     ofm_tens.mem_area = fast_storage_mem_area
                     ofm_tens.mem_type = fast_storage_type
 
         # Collect live ranges from tensors
         memories_list = [(fast_storage_mem_area, set((MemType.Scratch, MemType.Scratch_fast)))]
         lr_graph = live_range.LiveRangeGraph()
         for mem_area, mem_type_set in memories_list:
-            live_range.extract_live_ranges_from_cascaded_passes(
-                self.nng.get_root_subgraph(),
+            live_range.extract_live_ranges_from_schedule(
+                self.sg,
                 mem_area,
                 mem_type_set,
                 lr_graph,
-                Tensor.AllocationQuantum,
             )
+
         max_mem_usage = lr_graph.get_temporal_memory_usage(fast_storage_mem_area)
 
         # If max_mem_usage does not exceed staging limit at any point all lrs fit and can stay in fast storage
         if max(max_mem_usage) <= staging_limit:
             return
 
         # Build up the base memory usage by removing the mem_usage of the lrs we previously moved to fast-storage
@@ -1378,60 +1393,14 @@
                 base_mem_usage,
                 self.scratched_fms,
                 competing_tens_access,
                 self.evicted_fms,
             )
         assert max(max_mem_usage) <= staging_limit, "Allocation exceeds staging limit"
 
-    def move_constant_data(self):
-        """Determine if data can be moved from permanent storage to another memory area. A move will generate a DMA
-        command in the high-level command stream"""
-        for sched_op in self.sched_ops:
-            parent_op = sched_op.parent_op
-            is_lut_used = any(inp.purpose == TensorPurpose.LUT for inp in parent_op.inputs)
-            max_ifm_shram_avail = (
-                (self.arch.available_shram_banks(is_lut_used) - self.arch.shram_reserved_output_banks)
-                * self.arch.shram_bank_size
-                // 2
-            )
-
-            for idx, tens in enumerate(parent_op.inputs):
-                if tens.mem_type not in (MemType.Scratch, MemType.Scratch_fast):
-                    # Tensor is in permanent storage
-                    # Only when permanent storage differs from feature map storage, there is a point moving the data
-                    if (
-                        tens.mem_area in self.arch.permanent_storage_mem_area
-                        and self.arch.permanent_storage_mem_area != self.arch.feature_map_storage_mem_area
-                    ) or tens.purpose == TensorPurpose.LUT:
-                        if tens.purpose == TensorPurpose.LUT or (
-                            # For elementwise broadcast
-                            tens.purpose == TensorPurpose.FeatureMap
-                            and sched_op.op_type.is_binary_elementwise_op()
-                            and tens.shape != []
-                            and sched_op.ifm.shape != sched_op.ofm.shape
-                            and parent_op.write_shape is None
-                            and tens.storage_size() > max_ifm_shram_avail
-                        ):
-                            only_vector_product_consumers = all(
-                                oper and oper.type.npu_block_type == NpuBlockType.VectorProduct
-                                for oper in tens.consumers()
-                            )
-
-                            if (not only_vector_product_consumers) or tens.purpose == TensorPurpose.LUT:
-                                new_tens = tens.clone_into_fast_storage(self.arch)
-                                if tens.purpose == TensorPurpose.LUT:
-                                    new_tens.mem_area = MemArea.Shram
-
-                                new_tens.consumer_list.append(parent_op)
-                                parent_op.inputs[idx] = new_tens
-                                # If the index is out of range, IFM and IFM2 are the same tensor
-                                # and pass inputs don't have duplicates
-                                if idx < len(sched_op.parent_ps.inputs):
-                                    sched_op.parent_ps.inputs[idx] = new_tens
-
     def print_schedule(self, schedule: Schedule):
         print(f"Schedule: '{schedule.name}'")
         for sched_op in self.sched_ops:
             if sched_op not in schedule.cost_map:
                 # Sub-schedule printing
                 continue
 
@@ -1448,14 +1417,39 @@
             print(f"\t\tSRAM Used: {mem_usage} bytes")
 
         print("\tCascades:")
         for i, cascade in enumerate(schedule.cascades.values()):
             print(f"\t\t{i}: {cascade.start} -> {cascade.end}, size: {cascade.mem_usage}")
 
 
+def _update_memory_snapshot_for_all_npu_graphs(
+    nng: Graph, arch: ArchitectureFeatures, schedulers, verbose_progress: bool = False
+):
+    mem_area = arch.fast_storage_mem_area
+    mem_type_set = set((MemType.Scratch, MemType.Scratch_fast))
+
+    # Collect live ranges for the full graph
+    # extract_live_ranges_from_cascaded_passes will start from the root sg and
+    # all sub graphs/cascaded passes will be visited and the correct time_index
+    # will be set for all the tensors.
+    lr_graph = live_range.LiveRangeGraph()
+    live_range.extract_live_ranges_from_cascaded_passes(
+        nng.get_root_subgraph(), mem_area, mem_type_set, lr_graph, Tensor.AllocationQuantum, verbose_progress
+    )
+    # Populate time-array with memory used by live ranges
+    temporal_usage = lr_graph.get_temporal_memory_usage(arch.fast_storage_mem_area)
+
+    # Update snapshot for all the npu sub graphs
+    # Not needed for the scheduler any longer but npu_performance
+    # is using this information so it must have the correct state
+    for sg in schedulers:
+        sg.schedule.memory_snapshot = temporal_usage
+        sg.schedule.fast_storage_peak_usage = max(temporal_usage, default=0)
+
+
 def _update_tensor_allocation(nng: Graph, arch: ArchitectureFeatures, options):
     """
     Creates live ranges and runs tensor allocator for the current schedule
     (i.e. sg.schedule for all subgraphs), returns the maximum memory usage
     and updates SchedulerOpInfo.mem_usage for all operations in the schedule.
     """
     root_sg = nng.get_root_subgraph()
@@ -1476,14 +1470,15 @@
             nng,
             root_sg,
             arch,
             mem_area,
             mem_type_set,
             tensor_allocator=options.tensor_allocator,
             verbose_allocation=options.verbose_allocation,
+            verbose_progress=options.verbose_progress,
             cpu_tensor_alignment=options.cpu_tensor_alignment,
             hillclimb_max_iterations=options.hillclimb_max_iterations,
         )
 
 
 class FastStorageComponentAllocator:
     MAX_EXHAUSTIVE_LIFE_RANGE = 20
@@ -1575,82 +1570,95 @@
                 self.keep(lr, min_mem)
                 if lr in evicted_fms:
                     evicted_fms.remove(lr)
 
 
 def schedule_passes(nng: Graph, arch: ArchitectureFeatures, options, scheduler_options: SchedulerOptions):
     """Entry point for the Scheduler"""
+    verbose_progress = scheduler_options.verbose_progress
     # Initialize CPU subgraphs
     schedulers = dict()
     # Initialize schedulers with max schedule. Only schedule NPU subgraphs
-    for sg in nng.subgraphs:
+    for sg_idx, sg in enumerate(nng.subgraphs):
+        progress_print(verbose_progress, "Processing subgraph", sg_idx, nng.subgraphs)
         if sg.placement != PassPlacement.Npu:
             # Create cascaded passes for CPU Ops
             cascaded_passes = []
-            for idx, ps in enumerate(sg.passes):
+            for pass_idx, ps in enumerate(sg.passes):
+                progress_print(verbose_progress, "Creating cascaded passes for CPU op", pass_idx, sg.passes)
                 cps = CascadedPass(
                     ps.name,
                     SchedulingStrategy.WeightStream,
                     ps.inputs,
                     [],
                     ps.outputs,
                     [ps],
                     ps.placement,
                     False,
                 )
 
-                cps.time = idx
+                cps.time = pass_idx
                 ps.cascade = cps
                 cascaded_passes.append(cps)
 
             sg.cascaded_passes = cascaded_passes
         else:
             # Npu subgraph - create schedule
             scheduler = Scheduler(nng, sg, arch, scheduler_options)
             schedulers[sg] = scheduler
 
+            progress_print(verbose_progress, "Creating scheduler representation")
             scheduler.create_scheduler_representation(arch)
             sg.sched_ops = scheduler.sched_ops
-            scheduler.move_constant_data()
 
             # Create the Max schedule template
             max_schedule_template = scheduler.create_initial_schedule()
             scheduler.max_schedule = max_schedule_template
 
+            progress_print(verbose_progress, "Creating optimised max schedule")
             # Create the optimimised Max schedule
             sg.schedule = max_schedule_template
             scheduler.update_op_memory_snapshot(max_schedule_template)
             opt_max_schedule = scheduler.propose_schedule_buffering(max_schedule_template, 1 << 32)
             sg.schedule = opt_max_schedule
             scheduler.update_op_memory_snapshot(opt_max_schedule)
 
+            progress_print(verbose_progress, "Creating minimal schedule")
             # Create Min schedule
             min_schedule = scheduler.propose_minimal_schedule()
             initial_sram_limit = scheduler_options.optimization_sram_limit
             if scheduler_options.optimization_strategy == OptimizationStrategy.Size:
                 initial_sram_limit = scheduler.min_memory_req
 
             # Build cascades for Min schedule
+            progress_print(verbose_progress, "Building cascades for minimal schedule")
             scheduler.build_cascades_for_min_schedule(min_schedule, max_schedule_template, initial_sram_limit)
             sg.schedule = min_schedule
             scheduler.update_op_memory_snapshot(min_schedule)
 
             if scheduler_options.optimization_strategy == OptimizationStrategy.Performance:
+                progress_print(verbose_progress, "Creating schedule optimized for performance")
                 # Create an optimized schedule
                 sg.schedule = scheduler.optimize_schedule(
                     min_schedule, opt_max_schedule, max_schedule_template, scheduler_options
                 )
                 scheduler.update_op_memory_snapshot(sg.schedule)
 
             scheduler.apply_schedule(sg.schedule)
             scheduler.use_fast_storage_for_feature_maps(sg.schedule, scheduler_options.optimization_sram_limit)
 
             if scheduler_options.optimization_strategy == OptimizationStrategy.Performance and scheduler.evicted_fms:
+                progress_print(verbose_progress, "Optimizing weight buffering size")
                 # It might be possible to gain performance by reducing
                 # weight buffer size and instead fit fms in fast storage
                 scheduler.optimize_weight_buffering_size(min_schedule, scheduler_options)
 
             if scheduler_options.verbose_schedule:
                 scheduler.print_schedule(sg.schedule)
 
+    progress_print(verbose_progress, "Update memory snapshot for all NPU graphs")
+    # Make a full live range calculation starting from the root sg
+    _update_memory_snapshot_for_all_npu_graphs(nng, arch, schedulers, verbose_progress)
+
+    progress_print(verbose_progress, "Update tensor allocation")
     # Evaluate schedule
     _update_tensor_allocation(nng, arch, options)
```

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/shape4d.py` & `ethos-u-vela-3.8.0/ethosu/vela/shape4d.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/softmax.py` & `ethos-u-vela-3.8.0/ethosu/vela/softmax.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,21 +20,21 @@
 # Contains SoftMax
 import math
 
 import numpy as np
 
 from . import fp_math
 from . import scaling
-from .api import NpuRoundingMode
 from .data_type import DataType
 from .debug_database import DebugDatabase
 from .operation import ActivationFunction
 from .operation import ExplicitScaling
 from .operation import Op
 from .operation import Operation
+from .operation import RoundingMode
 from .operation_util import create_add
 from .operation_util import create_clz
 from .operation_util import create_depthwise_maxpool
 from .operation_util import create_mul
 from .operation_util import create_reduce_sum
 from .operation_util import create_shl
 from .operation_util import create_shr
@@ -277,15 +277,15 @@
         sub_op.activation.min = -128 - ifm_exp.quantization.zero_point
         sub_op.activation.max = 127 - ifm_exp.quantization.zero_point
 
         # PASS 2 - SHR
         name = f"{self.op.name}_shr{pass_number}"
         shift = create_const_tensor(f"{name}_const", [1, 1, 1, 1], DataType.int32, [12], quantization=no_scale_quant)
         shr_op = create_shr(name, ifm_exp, shift, no_scale_quant, activation)
-        shr_op.rounding_mode = NpuRoundingMode.NATURAL
+        shr_op.rounding_mode = RoundingMode.HalfUp
         rescaled_exp = add_op_get_ofm(shr_op)
 
         # PASS 3 - Reduce sum
         sum_of_exp = add_op_get_ofm(
             create_reduce_sum(f"{self.op.name}_reduce_sum{pass_number}", rescaled_exp, no_scale_quant, activation)
         )
 
@@ -439,15 +439,15 @@
         # PASS 29 - Multiply
         scaled_exp = add_op_get_ofm(
             create_mul(f"{self.op.name}_mul{pass_number}", ifm_exp, scale_factor, two_scale_quant, activation2)
         )
 
         # PASS 30 - SHR
         shr30_op = Operation(Op.SHR, f"{self.op.name}_shr{pass_number}")
-        shr30_op.rounding_mode = NpuRoundingMode.NATURAL
+        shr30_op.rounding_mode = RoundingMode.HalfUp
         shr30_op.add_input_tensor(scaled_exp)
         shr30_op.add_input_tensor(right_shift)
         shr30_op.set_output_tensor(ofm)
         shr30_op.ifm_shapes.append(Shape4D(scaled_exp.shape))
         shr30_op.ifm_shapes.append(Shape4D(right_shift.shape))
         shr30_op.ofm_shapes.append(Shape4D(scaled_exp.shape))
         DebugDatabase.add_optimised(self.op, shr30_op)
```

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/stats_writer.py` & `ethos-u-vela-3.8.0/ethosu/vela/stats_writer.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/supported_operators_util.py` & `ethos-u-vela-3.8.0/ethosu/vela/supported_operators_util.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tensor.py` & `ethos-u-vela-3.8.0/ethosu/vela/tensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,62 +211,58 @@
 
 class QuantizationParameters:
     __slots__ = (
         "min",
         "max",
         "num_bits",
         "narrow_range",
-        "next_after",
         "scale_f32",
         "zero_point",
         "quant_min",
         "quant_max",
         "quant_dim",
     )
 
     def __init__(
         self,
         min: Union[float, np.ndarray, None] = None,
         max: Union[float, np.ndarray, None] = None,
         num_bits=None,
         narrow_range=None,
+        scale_f32: Union[float, np.ndarray, None] = None,
+        zero_point: Union[int, np.ndarray, None] = None,
     ):
         self.min = min
         self.max = max
 
         self.num_bits = num_bits
         self.narrow_range = narrow_range
 
-        # Use the 'next after' float value of scale_f32 when converting to scale and shift. It can be combined with
-        # natural rounding to perform rounding away from zero. This only affects the ofm scale and bias tensor, it has
-        # no affect on global scaling i.e. the ofm_scale register
-        self.next_after = False
-        self.scale_f32: Union[float, np.ndarray, None] = None
-        self.zero_point: Union[int, np.ndarray, None] = None
+        self.scale_f32: Union[float, np.ndarray, None] = scale_f32
+        self.zero_point: Union[int, np.ndarray, None] = zero_point
         self.quant_min: Optional[float] = None
         self.quant_max: Optional[float] = None
         self.quant_dim: Optional[int] = None
 
     def __str__(self):
         return (
             f"<nng.QuantizationParameters min={self.min}, max={self.max}, num_bits={self.num_bits}, "
-            f"scale={self.scale_f32}, zero_point={self.zero_point}, next={self.next_after}>"
+            f"scale={self.scale_f32}, zero_point={self.zero_point}>"
         )
 
     __repr__ = __str__
 
     def clone(self) -> "QuantizationParameters":
         res = QuantizationParameters()
         res.min = self.min
         res.max = self.max
 
         res.num_bits = self.num_bits
         res.narrow_range = self.narrow_range
 
-        res.next_after = self.next_after
         res.scale_f32 = self.scale_f32
         res.zero_point = self.zero_point
         res.quant_min = self.quant_min
         res.quant_max = self.quant_max
         res.quant_dim = self.quant_dim
         return res
 
@@ -329,15 +325,15 @@
         values is not None
         and shape != []  # values are not a scalar
         and isinstance(values[0], np.floating)
         and dtype.type == BaseType.Unsigned
     ):
         values = [float(v) for v in values]
 
-    const_tensor.values = np.array(values, dtype=dtype.as_numpy_type())
+    const_tensor.values = np.array(values).astype(dtype.as_numpy_type())
     # Operator
     const_op = Operation(Op.Const, name)
     const_op.set_output_tensor(const_tensor)
     const_op.set_ifm_ofm_shapes()
     return const_tensor
 
 
@@ -393,15 +389,15 @@
         "brick_size",
         "quantization",
         "weight_compressed_offsets",
         "element_size_bytes",
         "block_traversal",
         "equivalence_id",
         "src_tensor",
-        "needs_linear_format",
+        "force_linear_format",
         "ifm_write_protected",
     )
     AllocationQuantum = 16
 
     def __init__(self, shape: Shape, dtype: DataType, name: str):
         self.shape = shape
         self._original_shape = shape
@@ -440,21 +436,27 @@
         self.brick_size: Tuple = (1, 1, 1, 1)
         self.element_size_bytes: int = 0
 
         # quantization parameters
         self.quantization: Optional[QuantizationParameters] = None
         self.block_traversal: TensorBlockTraversal = TensorBlockTraversal.Default
 
-        self.needs_linear_format = True
+        # Keep track of whether the linear format should be enforced
+        self.force_linear_format: Optional[bool] = None
         self.ifm_write_protected = False
 
         # Reference to parent-tensor if this tensor is a clone
         self.src_tensor: Optional[Tensor] = None
 
     @property
+    def use_linear_format(self) -> bool:
+        """Return whether the tensor should use linear format or not."""
+        return self.force_linear_format in (True, None)
+
+    @property
     def original_shape(self):
         return self._original_shape
 
     @property
     def address(self) -> int:
         return TensorAddressMap.get_address_for_tens(self.equivalence_id, self.mem_type)
 
@@ -494,21 +496,21 @@
         res.bandwidth_shape = list(self.bandwidth_shape)
         if self.quantization is not None:
             res.quantization = self.quantization.clone()
 
         res.name = res.name + suffix
         res.ops = []
         res.consumer_list = []
+        res.src_tensor = self
 
         return res
 
-    def clone_into_fast_storage(self, arch) -> "Tensor":
-        res = self.clone(suffix="_fast_storage")
-        res.mem_area = arch.fast_storage_mem_area
-        res.mem_type = MemType.Scratch_fast
+    def clone_into_shram(self, arch) -> "Tensor":
+        res = self.clone(suffix="_shram")
+        res.mem_area = MemArea.Shram
         res.src_tensor = self
         return res
 
     def as_1D(self):
         self.shape = [np.prod(self.shape)]
         if self.values is not None:
             self.values = self.values.reshape(self.shape)
@@ -542,15 +544,15 @@
         try:
             shape_len = len(self.shape)
         except TypeError:
             pass
 
         if shape_len > 4:
             return
-        assert not (self.needs_linear_format and fmt == TensorFormat.NHCWB16)
+        assert not (self.use_linear_format and fmt == TensorFormat.NHCWB16)
         self.storage_rounding_quantum = arch.storage_rounding_quantums[self.format]
         self.storage_rounding_quantum = tuple(self.storage_rounding_quantum[-shape_len:])
         self.brick_size = arch.brick_sizes[self.format]
         self.brick_size = tuple(self.brick_size[-shape_len:])
         if self.shape is None:
             return
```

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tensor_allocation.py` & `ethos-u-vela-3.8.0/ethosu/vela/tensor_allocation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright 2020-2022 Arm Limited and/or its affiliates <open-source-office@arm.com>
+# SPDX-FileCopyrightText: Copyright 2020-2023 Arm Limited and/or its affiliates <open-source-office@arm.com>
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 # Licensed under the Apache License, Version 2.0 (the License); you may
 # not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -197,22 +197,24 @@
     arch,
     mem_area,
     mem_type_set,
     tensor_allocator=TensorAllocator.Greedy,
     lr_graph=None,
     cpu_tensor_alignment=Tensor.AllocationQuantum,
     hillclimb_max_iterations=None,
+    verbose_progress=False,
 ):
     # Allocates addresses to tensors, returns False if tensors could not be fit within max_size
     lrs = live_range.extract_live_ranges_from_cascaded_passes(
         sg,
         mem_area,
         mem_type_set,
         lr_graph=lr_graph,
         cpu_tensor_alignment=cpu_tensor_alignment,
+        verbose_progress=verbose_progress,
     )
     total_sz = 0
     if lrs.ranges:
         tens_alloc = tensor_allocator
         if tens_alloc == TensorAllocator.Greedy:
             total_sz = greedy_allocate_live_ranges(lrs, cpu_tensor_alignment)
             verify_allocation(lrs, cpu_tensor_alignment)
@@ -231,14 +233,15 @@
     nng,
     sg,
     arch,
     mem_area,
     mem_type_set,
     tensor_allocator=TensorAllocator.Greedy,
     verbose_allocation=False,
+    verbose_progress=False,
     lr_graph=None,
     cpu_tensor_alignment=Tensor.AllocationQuantum,
     hillclimb_max_iterations=None,
     max_size=None,
     dry_test=False,
 ):
     # Allocates addresses to tensors, returns False if tensors could not be fit within max_size
@@ -247,14 +250,15 @@
         arch,
         mem_area,
         mem_type_set,
         tensor_allocator=tensor_allocator,
         lr_graph=lr_graph,
         cpu_tensor_alignment=cpu_tensor_alignment,
         hillclimb_max_iterations=hillclimb_max_iterations,
+        verbose_progress=verbose_progress,
     )
 
     if lrs.ranges:
         alloc_ok = max_size is None or total_sz <= max_size
         if dry_test or not alloc_ok:
             # Dry test or allocation failed; undo allocation
             for lr in lrs.ranges.values():
```

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/test/extapi/test_extapi_create_payload.py` & `ethos-u-vela-3.8.0/ethosu/vela/test/extapi/test_extapi_create_payload.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/test/extapi/test_extapi_encode_bias.py` & `ethos-u-vela-3.8.0/ethosu/vela/test/extapi/test_extapi_encode_bias.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/test/extapi/test_extapi_encode_weights.py` & `ethos-u-vela-3.8.0/ethosu/vela/test/extapi/test_extapi_encode_weights.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/test/extapi/test_extapi_find_block_configs.py` & `ethos-u-vela-3.8.0/ethosu/vela/test/extapi/test_extapi_find_block_configs.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/test/extapi/test_extapi_generate_commands.py` & `ethos-u-vela-3.8.0/ethosu/vela/test/extapi/test_extapi_generate_commands.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/test/extapi/test_extapi_get_version.py` & `ethos-u-vela-3.8.0/ethosu/vela/test/extapi/test_extapi_get_version.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/test/test_architecture_allocator.py` & `ethos-u-vela-3.8.0/ethosu/vela/test/test_architecture_allocator.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/test/test_compiler_driver.py` & `ethos-u-vela-3.8.0/ethosu/vela/test/test_compiler_driver.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/test/test_fp_math.py` & `ethos-u-vela-3.8.0/ethosu/vela/test/test_fp_math.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/test/test_graph_optimiser.py` & `ethos-u-vela-3.8.0/ethosu/vela/test/test_graph_optimiser.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/test/test_hillclimb_allocation.py` & `ethos-u-vela-3.8.0/ethosu/vela/test/test_hillclimb_allocation.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/test/test_live_range.py` & `ethos-u-vela-3.8.0/ethosu/vela/test/test_live_range.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/test/test_lut.py` & `ethos-u-vela-3.8.0/ethosu/vela/test/test_lut.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,31 +32,31 @@
 from ethosu.vela.test import testutil
 
 
 def set_256_lut(op, key, arch):
     random.seed(key)
     values = random.choices(range(256), k=256)
     lut_tensor = create_const_tensor(op.name + "_lut", [1, 1, 1, 256], DataType.uint8, values, TensorPurpose.LUT)
-    scratch_lut_tensor = lut_tensor.clone_into_fast_storage(arch)
+    scratch_lut_tensor = lut_tensor.clone_into_shram(arch)
     op.set_activation_lut(scratch_lut_tensor)
 
 
 def set_1K_lut(op, key, arch):
     random.seed(key)
     values = random.choices(range(256), k=256)
     lut_tensor = create_const_tensor(op.name + "_lut", [1, 1, 1, 256], DataType.int32, values, TensorPurpose.LUT)
-    scratch_lut_tensor = lut_tensor.clone_into_fast_storage(arch)
+    scratch_lut_tensor = lut_tensor.clone_into_shram(arch)
     op.set_activation_lut(scratch_lut_tensor)
 
 
 def set_2K_lut(op, key, arch):
     random.seed(key)
     values = random.choices(range(512), k=512)
     lut_tensor = create_const_tensor(op.name + "_lut", [1, 1, 1, 512], DataType.int32, values, TensorPurpose.LUT)
-    scratch_lut_tensor = lut_tensor.clone_into_fast_storage(arch)
+    scratch_lut_tensor = lut_tensor.clone_into_shram(arch)
     op.set_activation_lut(scratch_lut_tensor)
 
 
 def process(arch, op_list):
     # Returns subgraph with given operations
     nng = Graph()
     sg = testutil.create_subgraph(op_list)
```

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/test/test_model_reader.py` & `ethos-u-vela-3.8.0/ethosu/vela/test/test_model_reader.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/test/test_new_performance.py` & `ethos-u-vela-3.8.0/ethosu/vela/test/test_new_performance.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/test/test_nng_mapping.py` & `ethos-u-vela-3.8.0/ethosu/vela/test/test_nng_mapping.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/test/test_register_command_stream_util.py` & `ethos-u-vela-3.8.0/ethosu/vela/test/test_register_command_stream_util.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/test/test_scaling.py` & `ethos-u-vela-3.8.0/ethosu/vela/test/test_scaling.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/test/test_tensor_allocation.py` & `ethos-u-vela-3.8.0/ethosu/vela/test/test_tensor_allocation.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/test/test_tflite_model_semantic.py` & `ethos-u-vela-3.8.0/ethosu/vela/test/test_tflite_model_semantic.py`

 * *Files 2% similar despite different names*

```diff
@@ -498,15 +498,15 @@
 
 
 def test_mean_dtype():
     op = create_mean([1, 6, 6, 16], [1, 1, 1, 16], [1, 2], DataType.int8, {"keep_dims": True})
     assert semantic_checker.is_operator_semantic_valid(op)
     op.ifm.dtype = DataType.int16
     op.ofm.dtype = DataType.int16
-    assert not semantic_checker.is_operator_semantic_valid(op)
+    assert semantic_checker.is_operator_semantic_valid(op)
 
 
 def test_mean_axis():
     op = create_mean([1, 6, 6, 16], [1, 1, 1, 16], 0, DataType.int8, {"keep_dims": True})
     assert not semantic_checker.is_operator_semantic_valid(op)
     op = create_mean([1, 6, 6, 16], [1, 1, 1, 16], [3], DataType.int8, {"keep_dims": True})
     assert not semantic_checker.is_operator_semantic_valid(op)
@@ -572,7 +572,41 @@
     ifm.quantization = quant
     ofm = create_const_tensor("expand_dims_out", ofm_shape, DataType.uint8, np.zeros(ofm_shape))
     ofm.quantization = quant.clone()
     ofm.quantization.zero_point = 32
     dim = create_const_tensor("expand_dims_dim", [], DataType.uint8, 0)
     op = testutil.create_op(Op.ExpandDims, [ifm, dim], ofm, set_ifm_ofm_shapes=False)
     assert not semantic_checker.is_operator_semantic_valid(op)
+
+
+def test_lstm_semantics():
+    # Test valid configurations
+    op = testutil.create_lstm_op(3, 12, 24, 20, DataType.int8)
+    assert semantic_checker.is_operator_semantic_valid(op)
+    assert semantic_checker.is_operator_semantic_valid(testutil.create_lstm_op(3, 12, 24, 20, DataType.int16))
+    # Test invalid datatype
+    assert not semantic_checker.is_operator_semantic_valid(testutil.create_lstm_op(3, 12, 24, 20, DataType.uint8))
+    # Test invalid shape
+    ifm_shape = op.ifm.shape
+    ofm_shape = op.ofm.shape
+    op.ifm.shape = [12, 24]
+    assert not semantic_checker.is_operator_semantic_valid(op)
+    op.ifm.shape = ifm_shape
+    op.ofm.shape = [12, 20]
+    assert not semantic_checker.is_operator_semantic_valid(op)
+    op.ofm.shape = ofm_shape
+    # Test invalid number of intermediates
+    intermediate = op.intermediates.pop()
+    assert not semantic_checker.is_operator_semantic_valid(op)
+    op.intermediates.append(intermediate)
+    op.intermediates.append(intermediate)
+    assert not semantic_checker.is_operator_semantic_valid(op)
+    op.intermediates.pop()
+    # Test invalid number of inputs
+    input = op.inputs.pop()
+    assert not semantic_checker.is_operator_semantic_valid(op)
+    op.inputs.append(input)
+    op.inputs.append(input)
+    assert not semantic_checker.is_operator_semantic_valid(op)
+    op.inputs.pop()
+    # Test restored valid configuration
+    assert semantic_checker.is_operator_semantic_valid(op)
```

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/test/test_tflite_reader.py` & `ethos-u-vela-3.8.0/ethosu/vela/test/test_tflite_reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright 2020-2021 Arm Limited and/or its affiliates <open-source-office@arm.com>
+# SPDX-FileCopyrightText: Copyright 2020-2021, 2023 Arm Limited and/or its affiliates <open-source-office@arm.com>
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 # Licensed under the Apache License, Version 2.0 (the License); you may
 # not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -42,33 +42,33 @@
 
     @pytest.mark.parametrize("test_input,expected", len1_testdata)
     def test_len1_array_to_scalar(self, test_input, expected):
         output = TFLiteSubgraph.len1_array_to_scalar(test_input)
         assert output == expected
 
     parse_op_testdata = [
-        # op_type, opt_serializer, indices, inputs, output, expected
-        (Op.FullyConnected, None, TFLITE_IFM_WEIGHTS_BIAS_INDICES, [0, 1, 2], 3, 3),  # FC
-        (Op.FullyConnected, None, TFLITE_IFM_WEIGHTS_BIAS_INDICES, [0, 1, -1], 3, 3),  # FC disabled Bias
-        (Op.FullyConnected, None, TFLITE_IFM_WEIGHTS_BIAS_INDICES, [0, 1], 3, 3),  # FC no Bias
-        (Op.Conv2DBias, None, TFLITE_IFM_WEIGHTS_BIAS_INDICES, [2, 1, 3], 0, 3),  # Conv2D
-        (Op.Conv2DBackpropInput, None, TFLITE_CONV2D_BACKPROP_INDICES, [0, 1, 2, 3], 4, 4),  # TransposeConv
-        (Op.Conv2DBackpropInput, None, TFLITE_CONV2D_BACKPROP_INDICES, [0, 1, 2], 4, 4),  # TransposeConv no Bias
+        # op_type, opt_serializer, indices, version, inputs, output, expected
+        (Op.FullyConnected, None, TFLITE_IFM_WEIGHTS_BIAS_INDICES, 1, [0, 1, 2], 3, 3),  # FC
+        (Op.FullyConnected, None, TFLITE_IFM_WEIGHTS_BIAS_INDICES, 1, [0, 1, -1], 3, 3),  # FC disabled Bias
+        (Op.FullyConnected, None, TFLITE_IFM_WEIGHTS_BIAS_INDICES, 5, [0, 1], 3, 3),  # FC no Bias
+        (Op.Conv2DBias, None, TFLITE_IFM_WEIGHTS_BIAS_INDICES, 5, [2, 1, 3], 0, 3),  # Conv2D
+        (Op.Conv2DBackpropInput, None, TFLITE_CONV2D_BACKPROP_INDICES, 5, [0, 1, 2, 3], 4, 4),  # TransposeConv
+        (Op.Conv2DBackpropInput, None, TFLITE_CONV2D_BACKPROP_INDICES, 5, [0, 1, 2], 4, 4),  # TransposeConv no Bias
         pytest.param(
-            Op.Conv2DBias, None, TFLITE_IFM_WEIGHTS_BIAS_INDICES, [0, -1, 1], 3, 3, marks=pytest.mark.xfail
+            Op.Conv2DBias, None, TFLITE_IFM_WEIGHTS_BIAS_INDICES, 5, [0, -1, 1], 3, 3, marks=pytest.mark.xfail
         ),  # Conv2D no Weights
     ]
 
-    @pytest.mark.parametrize("op_type, opt_serializer, indices, inputs, output, expected", parse_op_testdata)
-    def test_parse_operator(self, op_type, opt_serializer, indices, inputs, output, expected):
+    @pytest.mark.parametrize("op_type, opt_serializer, indices, version, inputs, output, expected", parse_op_testdata)
+    def test_parse_operator(self, op_type, opt_serializer, indices, version, inputs, output, expected):
         with patch.object(TFLiteSubgraph, "__init__", lambda self, graph, subraph: None):
             # Mock a TFLiteSubGraph
             sg = TFLiteSubgraph(None, None)
             sg.graph = MagicMock()
-            sg.graph.operator_codes = [(op_type, opt_serializer, "", indices)]
+            sg.graph.operator_codes = [(op_type, opt_serializer, "", indices, version)]
 
             # Mock a couple of tensors
             sg.tensors = [MagicMock() for _ in range(5)]
             for i, tens in enumerate(sg.tensors):
                 tens.name = "tensor_{}".format(i)
                 tens.ops = []
```

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/test/test_tflite_supported_operators.py` & `ethos-u-vela-3.8.0/ethosu/vela/test/test_tflite_supported_operators.py`

 * *Files 18% similar despite different names*

```diff
@@ -105,23 +105,23 @@
     assert support.is_operator_supported(op)
 
 
 @pytest.mark.parametrize(
     "stride_w, stride_h, supported",
     [
         [0, 20, False],
-        [4, 1, True],
-        [4, 2, True],
-        [2, 2, True],
-        [4, 4, False],
+        [20, 0, False],
+        [4, 3, True],
         [4, 5, False],
-        [5, 4, False],
+        [4, 9, False],
         [3, 3, True],
         [1, 1, True],
-        [2, 4, False],
+        [20, 2, True],
+        [6, 3, True],
+        [8, 1, True],
     ],
 )
 def test_constraint_stride_range(stride_w: int, stride_h: int, supported: bool):
     # Stride width and height must lie within a certain range
     op = testutil.create_op_with_quant_tensors(Op.Conv2DBias, [1, 8, 8, 8], [1, 8, 8, 8], [1, 1, 1, 1])
     op.attrs = {"stride_w": stride_w, "stride_h": stride_h}
     assert support.is_operator_supported(op) == supported
@@ -614,12 +614,51 @@
 def test_mean_hw_product():
     op = create_mean([1, 64, 64, 16], [1, 16], [1, 2], DataType.uint8, {})
     assert support.is_operator_supported(op)
     op = create_mean([1, 65, 64, 16], [1, 1, 1, 16], [1, 2], DataType.int8, {"keep_dims": True})
     assert not support.is_operator_supported(op)
 
 
-def test_mean_hw_product_avgpool():
-    op = create_mean([1, 200, 200, 16], [1, 16], [1, 2], DataType.uint8, {"keep_dims": False})
+def test_lstm_support():
+    # Test valid configuration
+    op = testutil.create_lstm_op(3, 12, 24, 20, DataType.int8)
     assert support.is_operator_supported(op)
-    op = create_mean([1, 200, 200, 16], [1, 1, 1, 16], [1, 2], DataType.int8, {"keep_dims": True})
+    # Test CIFG not supported
+    input_to_input_weights, recurrent_to_input_weights = op.inputs[1], op.inputs[5]
+    op.inputs[1] = None
     assert not support.is_operator_supported(op)
+    op.inputs[1] = input_to_input_weights
+    op.inputs[5] = None
+    assert not support.is_operator_supported(op)
+    op.inputs[5] = recurrent_to_input_weights
+    # Test Peephole not supported
+    op.inputs[9] = input_to_input_weights
+    assert not support.is_operator_supported(op)
+    op.inputs[9] = None
+    op.inputs[10] = input_to_input_weights
+    assert not support.is_operator_supported(op)
+    op.inputs[10] = None
+    op.inputs[11] = input_to_input_weights
+    assert not support.is_operator_supported(op)
+    op.inputs[11] = None
+    # Test Projection not supported
+    op.inputs[16] = input_to_input_weights
+    assert not support.is_operator_supported(op)
+    op.inputs[16] = None
+    op.inputs[17] = input_to_input_weights
+    assert not support.is_operator_supported(op)
+    op.inputs[17] = None
+    # Test Normalisation not supported
+    op.inputs[20] = input_to_input_weights
+    assert not support.is_operator_supported(op)
+    op.inputs[20] = None
+    op.inputs[21] = input_to_input_weights
+    assert not support.is_operator_supported(op)
+    op.inputs[21] = None
+    op.inputs[22] = input_to_input_weights
+    assert not support.is_operator_supported(op)
+    op.inputs[22] = None
+    op.inputs[23] = input_to_input_weights
+    assert not support.is_operator_supported(op)
+    op.inputs[23] = None
+    # Test restored valid configuration
+    assert support.is_operator_supported(op)
```

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/ATan2Options.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/ATan2Options.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/AbsOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/AbsOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/AddNOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/AddNOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/AddOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/AddOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/ArgMaxOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/ArgMaxOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/ArgMinOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/ArgMinOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/AssignVariableOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/AssignVariableOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/BatchMatMulOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/BatchMatMulOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/BatchToSpaceNDOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/BatchToSpaceNDOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/BidirectionalSequenceLSTMOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/BidirectionalSequenceLSTMOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/BidirectionalSequenceRNNOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/BidirectionalSequenceRNNOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/BroadcastToOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/BroadcastToOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/BucketizeOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/BucketizeOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/Buffer.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/Buffer.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/BuiltinOperator.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/BuiltinOperator.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/BuiltinOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/BuiltinOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/CallOnceOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/CallOnceOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/CallOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/CallOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/CastOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/CastOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/ConcatEmbeddingsOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/ConcatEmbeddingsOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/ConcatenationOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/ConcatenationOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/Conv2DOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/Conv2DOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/Conv3DOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/Conv3DOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/CosOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/CosOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/CumsumOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/CumsumOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/CustomQuantization.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/CustomQuantization.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/DensifyOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/DensifyOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/DepthToSpaceOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/DepthToSpaceOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/DepthwiseConv2DOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/DepthwiseConv2DOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/DequantizeOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/DequantizeOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/DimensionMetadata.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/DimensionMetadata.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/DivOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/DivOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/DynamicUpdateSliceOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/DynamicUpdateSliceOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/EmbeddingLookupSparseOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/EmbeddingLookupSparseOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/EqualOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/EqualOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/ExpOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/ExpOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/ExpandDimsOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/ExpandDimsOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/FakeQuantOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/FakeQuantOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/FillOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/FillOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/FloorDivOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/FloorDivOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/FloorModOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/FloorModOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/FullyConnectedOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/FullyConnectedOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/GatherNdOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/GatherNdOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/GatherOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/GatherOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/GeluOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/GeluOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/GreaterEqualOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/GreaterEqualOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/GreaterOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/GreaterOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/HardSwishOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/HardSwishOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/HashtableFindOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/HashtableFindOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/HashtableImportOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/HashtableImportOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/HashtableOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/HashtableOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/HashtableSizeOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/HashtableSizeOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/IfOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/IfOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/Int32Vector.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/Int32Vector.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/L2NormOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/L2NormOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/LSHProjectionOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/LSHProjectionOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/LSTMOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/LSTMOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/LeakyReluOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/LeakyReluOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/LessEqualOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/LessEqualOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/LessOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/LessOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/LocalResponseNormalizationOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/LocalResponseNormalizationOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/LogSoftmaxOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/LogSoftmaxOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/LogicalAndOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/LogicalAndOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/LogicalNotOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/LogicalNotOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/LogicalOrOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/LogicalOrOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/MatrixDiagOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/MatrixDiagOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/MatrixSetDiagOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/MatrixSetDiagOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/MaximumMinimumOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/MaximumMinimumOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/Metadata.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/Metadata.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/MirrorPadOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/MirrorPadOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/Model.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/Model.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/MulOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/MulOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/NegOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/NegOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/NonMaxSuppressionV4Options.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/NonMaxSuppressionV4Options.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/NonMaxSuppressionV5Options.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/NonMaxSuppressionV5Options.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/NotEqualOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/NotEqualOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/OneHotOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/OneHotOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/Operator.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/Operator.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/OperatorCode.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/OperatorCode.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/PackOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/PackOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/PadOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/PadOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/PadV2Options.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/PadV2Options.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/Pool2DOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/Pool2DOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/PowOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/PowOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/QuantizationParameters.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/QuantizationParameters.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/QuantizeOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/QuantizeOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/RNNOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/RNNOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/RandomOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/RandomOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/RangeOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/RangeOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/RankOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/RankOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/ReadVariableOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/ReadVariableOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/ReducerOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/ReducerOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/ReshapeOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/ReshapeOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/ResizeBilinearOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/ResizeBilinearOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/ResizeNearestNeighborOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/ResizeNearestNeighborOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/ReverseSequenceOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/ReverseSequenceOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/ReverseV2Options.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/ReverseV2Options.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/Rfft2dOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/Rfft2dOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/SVDFOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/SVDFOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/ScatterNdOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/ScatterNdOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/SegmentSumOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/SegmentSumOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/SelectOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/SelectOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/SelectV2Options.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/SelectV2Options.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/SequenceRNNOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/SequenceRNNOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/ShapeOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/ShapeOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/SignOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/SignOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/SignatureDef.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/SignatureDef.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/SkipGramOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/SkipGramOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/SliceOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/SliceOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/SoftmaxOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/SoftmaxOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/SpaceToBatchNDOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/SpaceToBatchNDOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/SpaceToDepthOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/SpaceToDepthOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/SparseToDenseOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/SparseToDenseOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/SparsityParameters.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/SparsityParameters.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/SplitOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/SplitOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/SplitVOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/SplitVOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/SquareOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/SquareOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/SquaredDifferenceOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/SquaredDifferenceOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/SqueezeOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/SqueezeOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/StridedSliceOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/StridedSliceOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/SubGraph.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/SubGraph.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/SubOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/SubOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/Tensor.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/Tensor.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/TensorMap.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/TensorMap.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/TileOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/TileOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/TopKV2Options.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/TopKV2Options.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/TransposeConvOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/TransposeConvOptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,22 +45,32 @@
     # TransposeConvOptions
     def StrideH(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(8))
         if o != 0:
             return self._tab.Get(flatbuffers.number_types.Int32Flags, o + self._tab.Pos)
         return 0
 
-def TransposeConvOptionsStart(builder): builder.StartObject(3)
+    # TransposeConvOptions
+    def FusedActivationFunction(self):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(10))
+        if o != 0:
+            return self._tab.Get(flatbuffers.number_types.Int8Flags, o + self._tab.Pos)
+        return 0
+
+def TransposeConvOptionsStart(builder): builder.StartObject(4)
 def Start(builder):
     return TransposeConvOptionsStart(builder)
 def TransposeConvOptionsAddPadding(builder, padding): builder.PrependInt8Slot(0, padding, 0)
 def AddPadding(builder, padding):
     return TransposeConvOptionsAddPadding(builder, padding)
 def TransposeConvOptionsAddStrideW(builder, strideW): builder.PrependInt32Slot(1, strideW, 0)
 def AddStrideW(builder, strideW):
     return TransposeConvOptionsAddStrideW(builder, strideW)
 def TransposeConvOptionsAddStrideH(builder, strideH): builder.PrependInt32Slot(2, strideH, 0)
 def AddStrideH(builder, strideH):
     return TransposeConvOptionsAddStrideH(builder, strideH)
+def TransposeConvOptionsAddFusedActivationFunction(builder, fusedActivationFunction): builder.PrependInt8Slot(3, fusedActivationFunction, 0)
+def AddFusedActivationFunction(builder, fusedActivationFunction):
+    return TransposeConvOptionsAddFusedActivationFunction(builder, fusedActivationFunction)
 def TransposeConvOptionsEnd(builder): return builder.EndObject()
 def End(builder):
     return TransposeConvOptionsEnd(builder)
```

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/TransposeOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/TransposeOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/Uint16Vector.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/Uint16Vector.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/Uint8Vector.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/Uint8Vector.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/UnidirectionalSequenceLSTMOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/UnidirectionalSequenceLSTMOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/UniqueOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/UniqueOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/UnpackOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/UnpackOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/UnsortedSegmentMaxOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/UnsortedSegmentMaxOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/UnsortedSegmentMinOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/UnsortedSegmentMinOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/UnsortedSegmentProdOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/UnsortedSegmentProdOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/UnsortedSegmentSumOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/UnsortedSegmentSumOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/VarHandleOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/VarHandleOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/VariantSubType.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/VariantSubType.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/WhereOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/WhereOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/WhileOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/WhileOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite/ZerosLikeOptions.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite/ZerosLikeOptions.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite_graph_optimiser.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite_graph_optimiser.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,48 +13,58 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # Description:
 # Early optimisation of a TensorFlow Lite based network graph, using the rewrite_graph module
 # to do the traversal of the graph.
+from __future__ import annotations
+
 import math
 import uuid
 
 import numpy as np
 
 from . import fp_math
 from . import rewrite_graph
 from . import scaling
-from .api import NpuRoundingMode
 from .data_type import BaseType
 from .data_type import DataType
 from .debug_database import DebugDatabase
 from .errors import UnsupportedFeatureError
 from .ethos_u55_regs.ethos_u55_regs import resampling_mode
 from .graph_optimiser_util import bypass_memory_only_ops
 from .graph_optimiser_util import calc_explicit_padding
 from .graph_optimiser_util import convert_depthwise_to_conv
-from .graph_optimiser_util import convert_to_lut
-from .graph_optimiser_util import fix_sg_input_output
+from .graph_optimiser_util import create_avg_pool_for_concat
 from .graph_optimiser_util import memory_only_ops
 from .graph_optimiser_util import move_splitsliceread_to_consumer
 from .graph_optimiser_util import needed_total_padding
 from .graph_optimiser_util import set_ifm_ofm_op_shapes
 from .graph_optimiser_util import set_tensor_equivalence
+from .lstm import Lstm
+from .lut import convert_to_lut
+from .lut import create_lut_8bit_op
+from .lut import create_lut_int16_op
 from .numeric_util import clamp_sigmoid
+from .numeric_util import full_shape
 from .numeric_util import round_away_zero
+from .numeric_util import round_down_log2
 from .operation import create_activation_function
 from .operation import ExplicitScaling
 from .operation import NpuBlockType
 from .operation import Op
 from .operation import Operation
 from .operation import Padding
+from .operation import RoundingMode
 from .operation_util import create_add_nop
 from .operation_util import create_avgpool_nop
+from .operation_util import create_cast_op
+from .operation_util import create_depthwise_maxpool
+from .operation_util import create_memcpy
 from .operation_util import get_pad_values_from_input
 from .scaling import quantise_scale
 from .shape4d import Shape4D
 from .softmax import SoftMax
 from .tensor import check_quantized_tens_scaling_equal
 from .tensor import create_const_tensor
 from .tensor import create_equivalence_id
@@ -62,31 +72,14 @@
 from .tensor import Tensor
 from .tensor import TensorPurpose
 from .tflite_mapping import optype_to_builtintype
 
 passthrough_nodes = (Op.Identity,)
 
 
-def create_avg_pool_for_concat(concat_op, name, ifm, ifm_shape: Shape4D, write_offset: Shape4D):
-    """Creates an average pool for the given concat op/input feature map"""
-    ofm = concat_op.ofm
-    avgpool_op = create_avgpool_nop(name)
-    avgpool_op.inputs = [ifm]
-    avgpool_op.outputs = [ofm]
-
-    avgpool_op.write_offset = write_offset
-    avgpool_op.write_shape = ifm_shape
-    ofm.ops.append(avgpool_op)
-    avgpool_op.ifm_shapes.append(ifm_shape)
-    avgpool_op.ofm_shapes.append(concat_op.ofm_shapes[0])
-    avgpool_op.memory_function = Op.ConcatSliceWrite
-    DebugDatabase.add_optimised(concat_op, avgpool_op)
-    return avgpool_op
-
-
 def remove_passthrough_tensor(tens, arch, nng):
     if len(tens.ops) == 1 and tens.ops[0].type in passthrough_nodes:
         assert len(tens.ops[0].inputs) == 1
         tens = tens.ops[0].inputs[0]
     return tens
 
 
@@ -189,25 +182,23 @@
 
     return tens
 
 
 def remove_SplitSliceRead(op, arch):
 
     if op.type == Op.SplitSliceRead:
-        # Check if it is possible to put the SplitSliceRead on the tensor consumer, or if an avgpool need to be inserted
-        if (
-            len(op.ofm.consumer_list) == 1
-            and op.ofm.consumer_list[0] is not None
-            and op.ofm.consumer_list[0].run_on_npu
-            and op.ofm.consumer_list[0].type not in memory_only_ops
-            and op.ofm_shapes[0] == Shape4D.from_list(op.ofm.shape)
+        # Check if it is possible to put the SplitSliceRead on the tensor consumer(s),
+        # or if an avgpool need to be inserted
+        if op.ofm_shapes[0] == Shape4D.from_list(op.ofm.shape) and all(
+            consumer is not None and consumer.run_on_npu and consumer.type not in memory_only_ops
+            for consumer in op.ofm.consumer_list
         ):
-            # SplitSliceRead can be performed by tensor consumer
-            cons_op = op.ofm.consumer_list[0]
-            move_splitsliceread_to_consumer(op, cons_op)
+            # SplitSliceRead can be performed by tensor consumer(s)
+            for cons_op in list(op.ofm.consumer_list):
+                move_splitsliceread_to_consumer(op, cons_op)
         else:
             avgpool_op = create_avgpool_nop(op.name + "_avgpool")
             avgpool_op.add_input_tensor(op.ifm)
             avgpool_op.outputs = [op.ofm]
             op.ofm.ops.remove(op)
             op.ofm.ops.append(avgpool_op)
             avgpool_op.ifm_shapes.append(op.ifm_shapes[0])
@@ -300,15 +291,15 @@
     op.set_input_tensor(create_const_tensor(name, shape, dtype, values, quantization=quantization), 0)
     op.set_ifm_ofm_shapes()
     DebugDatabase.add_optimised(op, op)
 
     return op
 
 
-# Convert ResizeNearestNeightbor with align corners to a depthwise convolution. The IFM will already have been upscaled
+# Convert ResizeNearestNeighbor with align corners to a depthwise convolution. The IFM will already have been upscaled
 # apart from the final x2 scaling which will be done as part of this operation. The kernel contains a single coefficient
 # to select the appropriate nearest neighbor value
 def convert_resizenn_ac_to_depthwise_conv(op, upscale_factor):
     ifm = op.ifm
     ofm = op.ofm
     output_depth = ofm.shape[-1]
     dw_op_attrs = {
@@ -319,15 +310,15 @@
         "depth_multiplier": 1,
         "channel_multiplier": 1,
         "dilation_h_factor": 1,
         "dilation_w_factor": 1,
         "dilation": (1, 1, 1, 1),
     }
 
-    # change resizebilinear to depthwise
+    # change ResizeNearestNeighbor to Depthwise
     op.type = Op.DepthwiseConv2DBias
     op.attrs.update(dw_op_attrs)
     op.set_input_tensor(ifm, 0)  # ifm tensor index
     op.activation = None
 
     # add input resample to resize by x2
     op.ifm_resampling_mode = resampling_mode.NEAREST
@@ -457,14 +448,186 @@
     scaled_op.outputs[0].ops = [scaled_op]
     scaled_op.set_ifm_ofm_shapes()
     DebugDatabase.add_optimised(op, scaled_op)
 
     return op
 
 
+def convert_argmax_to_depthwise_conv_and_max_pool(op, arch, nng):
+    """
+    Convert ArgMax to DWConv2D->MaxPool->DWConv2D, see details below.
+
+    Example:
+    arr = [4,   [00000100,
+           6, =  00000110,  # <-- This is the largest value, so we're expecting argmax(arr) = 1
+           5]    00000101]
+
+    Use 16-bit precision and shift all values 7 bits to the left:
+    Shifted_arr = [0000001000000000,
+                   0000001100000000,
+                   0000001010000000]
+
+    Add "c - index of channel" to each channel:
+    Shifted_arr_plus_reverse_idx = [0000001000000010, (+2)
+                                    0000001100000001, (+1)
+                                    0000001010000000] (+0)
+
+    The index is reversed since ArgMax selects the lowest index if maximum value is found at two index. The index will
+    act as a tie-breaker between channels with equal values and since we want the smallest channel index to be chosen
+    we reverse the index before the maxpool and then subtract the index from the number of channel after the maxpool to
+    get the correct index.
+
+    Find the maximum value in the array:
+    val = max(shifted_arr_plus_reverse_idx) = 0000001100000001
+
+    Subtract the value from the number of channels:
+    shifted_arr_plus_idx = (c-1) - val = 2 - 1 = 1
+
+    Extract the 7 lowest bits using a LUT to cut off the 9 most significant bits:
+    idx = LUT(val) = 0000000000000001 = 1
+    """
+
+    if op.type == Op.ArgMax:
+        ifm, ofm = op.inputs[0], op.outputs[0]
+        identity_quant = QuantizationParameters()
+        identity_quant.zero_point = 0
+        identity_quant.scale_f32 = 1.0
+        # Add last dimension to ofm shape
+        ofm.shape += [1]
+        ofm.ops = []
+
+        # Create 1x1 Depthwise convolution with 2**7 weights for each channel to convert precision to 16 bit and shift
+        # all values 7 bits to the left
+        # Set necessary depthwise attributes
+        dw_op_attrs = {
+            "padding": Padding.VALID,
+            "stride_h": 1,
+            "stride_w": 1,
+            "strides": (1, 1, 1, 1),
+            "depth_multiplier": 1,
+            "channel_multiplier": 1,
+            "dilation_h_factor": 1,
+            "dilation_w_factor": 1,
+            "dilation": (1, 1, 1, 1),
+            "explicit_padding": None,
+        }
+        orig_name = op.name
+        op.name = f"{orig_name}_depthwise_conv_SHL_7"
+        op.type = Op.DepthwiseConv2DBias
+        op.attrs.update(dw_op_attrs)
+        n, h, w, c = full_shape(4, ifm.shape, 1)
+        shape = [1, 1, 1, c]
+        kernel = np.dstack([2**7] * c)
+        op.inputs = []
+        op.add_input_tensor(ifm)
+        op.add_input_tensor(
+            create_const_tensor(
+                "weights",
+                shape,
+                DataType.uint8,
+                np.array(kernel).reshape(shape),
+                quantization=identity_quant,
+            ),
+        )
+        # Let the bias for each channel be the "reverse" index of the channel it is in, ie c - channel_idx
+        reverse_idxs = list(reversed(range(c)))
+        bias_tensor = create_const_tensor(op.name + "_bias", [c], DataType.int64, reverse_idxs)
+        op.add_input_tensor(bias_tensor)
+
+        intermediate_tens = Tensor([n, h, w, c], DataType.int16, "int16_and_shifted_7_bits_left")
+        intermediate_tens.quantization = ifm.quantization
+        op.set_output_tensor(intermediate_tens)
+        op.set_ifm_ofm_shapes()
+        orig_ifm_shape = op.ifm_shapes[0]
+        DebugDatabase.add_optimised(op, op)
+
+        # To extract 7 least significant bits and swap reverse index back to real index using a LUT activation, we set
+        # the base value to c-1 and slope to -128. The 16-bit LUT uses a table of 32-bit values where the top 16 bits
+        # represent the slope and bottom 16 bits the base which are used to interpolate the activation value.
+        slope = (-128 & 0xFFFF) << 16  # Top 16 bits of 32 bit LUT table value
+        base = c - 1  # Bottom 16 bits of the LUT table value
+        lut_tensor = create_const_tensor(
+            "maxpool_LUT_extract_7_LSB",
+            [1, 1, 1, 512],
+            DataType.uint32,
+            [slope + base] * 512,
+            TensorPurpose.LUT,
+        )
+
+        # Split large feature maps into smaller chunks since the Depthwise Maxpool height dimension can overflow due to
+        # flattening the ifm to (H*W)xCx1
+        max_height = 2**16 // orig_ifm_shape.width
+        num_full_height_ops = orig_ifm_shape.height // max_height
+        last_op_height = orig_ifm_shape.height - max_height * num_full_height_ops
+        op_heights = [max_height] * num_full_height_ops
+        if last_op_height > 0:
+            op_heights.append(last_op_height)
+
+        # Create maxpool output tensor which is reshaped to 1x(H*W)x1x1. The product H*W might be larger than the
+        # maximum allowed height, but that's handled by reading and writing the data in chunks
+        maxpool_ofm = Tensor([1, orig_ifm_shape.height * orig_ifm_shape.width, 1, 1], DataType.int16, "argmax_maxpool")
+        maxpool_ofm.quantization = identity_quant
+
+        for op_idx, op_height in enumerate(op_heights):
+            maxpool_op = create_depthwise_maxpool(
+                f"dw_maxpool_{op_idx}", intermediate_tens, orig_ifm_shape, identity_quant
+            )
+            maxpool_op.outputs = [maxpool_ofm]
+            maxpool_ofm.ops.append(maxpool_op)
+            maxpool_op.ofm_shapes = [Shape4D(maxpool_ofm.shape)]
+            maxpool_op.set_activation_lut(lut_tensor)
+
+            # Set read and write shapes/offsets to read/write chunks of the IFM/OFM
+            maxpool_op.read_shapes[0] = Shape4D([1, op_height * orig_ifm_shape.width, orig_ifm_shape.depth, 1])
+            maxpool_op.read_offsets[0] = Shape4D([0, sum(op_heights[:op_idx]) * orig_ifm_shape.width, 0, 0])
+            maxpool_op.write_shape = Shape4D([1, op_height * orig_ifm_shape.width, 1, 1])
+            maxpool_op.write_offset = Shape4D([0, sum(op_heights[:op_idx]) * orig_ifm_shape.width, 0, 0])
+            DebugDatabase.add_optimised(op, maxpool_op)
+
+        # Set final shape
+        maxpool_ofm.set_all_shapes([1, h, w, 1])
+
+        # Convert 16bit to 32bit or 64bit
+        if ofm.dtype == DataType.int64:
+            # If OFM dtype is int64 the result is converted by two cast ops (16bit to 32bit)
+            #
+            #   A     -> B         -> C          -> D (OFM)
+            #   |0001|   |00010000|   |0001|0000|   |00010000|00000000|
+            #    i16      i32          i16  i16      i32      i32
+            #                                       <-------i64------->
+            #
+            #   Memcpy is used to copy the content from B to C and from D to OFM
+            #   Memcpy will be turned into a nop or an DMA transer if memory regions differs.
+            intermediate_32bit = Tensor([1, h, w, 1], DataType.int32, f"{orig_name}_32bit")
+        else:
+            intermediate_32bit = ofm
+
+        op_cast = create_cast_op(f"{orig_name}_cast_to_32bit_1", maxpool_ofm, intermediate_32bit)
+        DebugDatabase.add_optimised(op, op_cast)
+
+        if ofm.dtype == DataType.int64:
+            # Create int16 tensor with double shape to cover the intermediate_32bit result from the first cast
+            intermediate_16bit_2x_size = Tensor([1, h, w, 2], DataType.int16, f"{orig_name}_16bit_2x_size")
+            memcpy_op = create_memcpy(f"{orig_name}_memcpy_1", intermediate_32bit, intermediate_16bit_2x_size)
+            DebugDatabase.add_optimised(op, memcpy_op)
+
+            # Create int32 tensor with double ofm shape to be able to store a "int64" result
+            intermediate_32bit_2x_size = Tensor([1, h, w, 2], DataType.int32, f"{orig_name}_32bit_2x_size")
+
+            op_cast = create_cast_op(
+                f"{orig_name}_cast_to_32bit_2", intermediate_16bit_2x_size, intermediate_32bit_2x_size
+            )
+            DebugDatabase.add_optimised(op, op_cast)
+
+            memcpy_op = create_memcpy("f{orig_name}_memcpy_2", intermediate_32bit_2x_size, ofm)
+            DebugDatabase.add_optimised(op, memcpy_op)
+
+    return op
+
+
 def convert_resizebilinear_to_depthwise_convolutions(op, half_pixel_centers=True):
     def _compute_interpolation_values(index, input_size, output_size):
         scale = input_size / output_size
         scaled_value = (index + 0.5 * half_pixel_centers) * scale - 0.5 * half_pixel_centers
         lower_bound = max(np.floor(scaled_value), 0)
 
         return scaled_value, lower_bound
@@ -528,20 +691,16 @@
         DebugDatabase.add_optimised(op, op)
 
         dw_conv = Operation(Op.DepthwiseConv2DBias, "depthwise_conv")
         dw_conv._original_type = Op.ResizeBilinear
         dw_conv.write_shape = Shape4D(n, h, w, c)
         dw_conv.write_offset = Shape4D(0, 0, 0, 0)
 
-        # Set the output rounding mode. Resize bilinear requires rounding away from zero. Therefore, we need to
-        # adjust the accumulated value by a "small" amount before applying natural rounding. The "small" amount
-        # should be big enough to cause a x.5 to be rounded correctly but small enough not to cause smaller
-        # values to be incorrectly rounded
-        ofm.quantization.next_after = True
-        dw_conv.rounding_mode = NpuRoundingMode.NATURAL
+        # Resize bilinear requires rounding away from zero
+        dw_conv.rounding_mode = RoundingMode.AwayZero
 
         # Double height and width stride to write the output of each of the four depthwise convolutions below
         # interleaved with each other when combined with OFM tile base offsets.
         dw_conv.ofm_stride_multiplier = [1, 2, 2]  # C/H/W
 
         # Choose tile padding direction - pad by 1 with edge values in two direction.
         # For example, TL (top left) will pad top and left in H/W-plane in all channels.
@@ -622,16 +781,17 @@
         # if it shouldn't, remove_passthrough_tensor will fail appropriately
         op.inputs = [i for i in op.inputs if i.shape == op.outputs[0].shape]
         op.type = Op.Identity
     return op
 
 
 def rewrite_fully_connected_input(op: Operation, arch, nng):
-
-    if op.type == Op.FullyConnected:
+    # If the operation already have a read shape do not modify
+    # the ifm shape, since that will already be correct
+    if op.type == Op.FullyConnected and not op.read_shapes[0]:
         new_shape = op.ifm.get_shape_as_2d(op.weights.shape[-2])
         assert new_shape is not None, "Tensor can not be reshaped to 2D"
         op.ifm_shapes[0] = new_shape
 
         if op.ifm_shapes[0].batch > 1 and op.ofm_shapes[0].batch == 1:
             # If IFM is batching then also make sure OFM is batching
             h, w = op.ofm_shapes[0].height, op.ofm_shapes[0].width
@@ -783,74 +943,162 @@
         weight_tensor.values = np.transpose(weight_tensor.values, (0, 1, 3, 2))
         weight_tensor.set_all_shapes(list(weight_tensor.values.shape))
         weight_tensor.weight_transpose_depthwise = True
 
     return op
 
 
-def fixup_strided_conv(op, arch, nng):
+def fixup_strided_conv(op: Operation, arch, nng) -> Operation:
+    """Optimize or fixup strided Conv2DBias
+    Optimization:
+        Reduce, when possible, the Conv2DBias stride from N with 1 > N > 4 to 1
+        by re-shaping both IFM and filter.
+
+    Fixup:
+        Introduce software support for Conv2DBias with stride_width > 4 by
+        reducing it to 1, 2 or 3 (HW supported strides) when possible by
+        re-shaping both IFM and filter.
+    """
     if op.type != Op.Conv2DBias:
         return op
     stride_x, stride_y = op.get_kernel_stride()
     weight_tensor = op.weights
     ifm_shape = op.ifm_shapes[0]
 
     # Do not optimize if op is not the first in the network and stride is
     # supported by the hardware
     if op.op_index != 0 and stride_x < 4:
         return op
-    op.ifm.needs_linear_format = True
 
-    if (
-        (stride_x == 2 or stride_x == 4)
-        and ifm_shape.depth <= 4
-        and ifm_shape.width % 2 == 0
-        and weight_tensor is not None
-        and weight_tensor.shape[1] >= 2
-    ):
+    def calc_resize_factor(ifm_width: int, stride_x: int) -> tuple[int, int]:
+        """Compute resize factor for strided Conv2D optimization"""
+        # Define strides that are supported by HW
+        hw_supported_strides = (2, 3)
+        resize_factor = stride_x
+
+        if ifm_width % resize_factor != 0:
+            # In case it is not divisible, check if the resize factor is
+            # divisible by any of the hw_supported_strides. If it is, re-compute
+            # the resize factor to be the value that leads us to
+            # reach a hw supported stride.
+            # E.g.: IFM width = 133, stride = 14, filter width = 7 can be
+            #       optimised to IFM width = 19, stride = 2, filter width = 7 using
+            #       a resize factor of 7. The final stride is 2 which is
+            #       supported by the hardware.
+            supported_final_strides = (x for x in hw_supported_strides if resize_factor % x == 0)
+            new_resize_factor = resize_factor // next(supported_final_strides, 1)
+            resize_factor = new_resize_factor if resize_factor != new_resize_factor else 1
+
+        optimised_stride = stride_x // resize_factor
+
+        return resize_factor, optimised_stride
+
+    resize_factor, final_stride = calc_resize_factor(ifm_shape.width, stride_x)
+
+    def calc_filter_padding(
+        ifm_padding_type: Padding | None,
+        ifm_current_padding_x: int,
+        post_op_stride: int,
+        opt_resize_factor: int,
+        filter_width: int,
+    ) -> tuple[int, int, int, int]:
+        """Calculate zero padding to be added to the filter.
+
+        Parameters
+        ----------
+        ifm_padding_type : Padding or None
+            The padding type that is applied to the IFM.
+        ifm_current_padding_x : int
+            Padding amount that is added to the IFM before optimization.
+        post_op_stride : int
+            The final stride once optimization is performed.
+        opt_resize_factor : int
+            The factor by which the stride will be reduced.
+            E.g. opt_resize_factor = 2 on a stride of 4 will produce
+            a stride of 2 after the optimization
+        filter_width : int
+            Width of the filter before optimization.
+
+        Returns
+        -------
+        padding : tuple[int, int, int, int]
+            A tuple with the ammount of padding on each side (top, left, bottom, right)
+        """
+        padding_size = 0
+        padding = (0, 0, 0, 0)
+        if ifm_padding_type and ifm_padding_type != Padding.VALID:
+            padding_size = (ifm_current_padding_x + post_op_stride) * opt_resize_factor - filter_width
+            # Distribute padding between left and right side of the filter
+            padding_left = padding_size // 2
+            padding = (0, padding_left, 0, padding_size - padding_left)
+
+        # Check if filter width is divisible by the stride width (required for optimization)
+        # If padding was already added above, the filter width is already divisible by
+        # resize factor, so this should be skipped.
+        if padding_size == 0 and filter_width % opt_resize_factor != 0:
+            padding_size = opt_resize_factor - (filter_width % opt_resize_factor)
+            # Add padding zeros to the right
+            padding = (0, 0, 0, padding_size)
+
+        return padding
+
+    # Compute the depth of the IFM once the strided Conv2D is optimised
+    post_opt_ifm_depth = ifm_shape.depth * resize_factor
+
+    if stride_x > 1 and (post_opt_ifm_depth <= 8 or stride_x > 3) and resize_factor != 1 and weight_tensor is not None:
         k_w, _ = op.get_kernel_size()
-        curr_padding_x = needed_total_padding(ifm_shape.width, stride_x, k_w)
-        optimised_padding_x = needed_total_padding(ifm_shape.width // stride_x, 1, (k_w + 1) // stride_x)
-        padding_type = op.attrs.get("padding", None)
+        weight_shape = weight_tensor.shape
 
-        # If padding is enabled, check if current padding matches optimised padding
-        if not padding_type or (padding_type != Padding.VALID and curr_padding_x != optimised_padding_x):
-            # Horizontal padding would become different after optimisation; this would not work
+        padding_type = op.attrs.get("padding", None)
+        if padding_type in (None, Padding.EXPLICIT, Padding.TILE):
             return op
-        # IFM
-        op.ifm_shapes[0] = Shape4D(
-            [ifm_shape.batch, ifm_shape.height, ifm_shape.width // stride_x, ifm_shape.depth * stride_x]
+        # Compute current padding as if IFM padding is SAME
+        curr_padding_x = needed_total_padding(ifm_shape.width, stride_x, k_w)
+        # Compute the padding needed on the filter for the optimisation
+        _, left_filter_padding, _, right_filter_padding = calc_filter_padding(
+            padding_type, curr_padding_x, final_stride, resize_factor, k_w
         )
+        total_horizontal_padding = left_filter_padding + right_filter_padding
+        # If IFM padding is enabled, check if pre-opt and post-opt padding is
+        # the same while taking into consideration the extra filter padding.
+        if padding_type == Padding.SAME:
+            optimised_padding_x = needed_total_padding(
+                ifm_shape.width // resize_factor, final_stride, (k_w + 1 + total_horizontal_padding) // resize_factor
+            )
+            if curr_padding_x != optimised_padding_x:
+                # Horizontal padding would become different after optimisation; this would not work
+                return op
 
-        # Weights
-        weight_shape = weight_tensor.shape
-        if weight_shape[1] % 2 != 0:
-            weight_shape[1] = weight_shape[1] + 1
-            padded_array = np.zeros(weight_shape)
-            for i in range(weight_shape[0]):
-                padded_array[i] = np.vstack(
-                    [
-                        weight_tensor.values[i],
-                        np.full((1, weight_shape[2], weight_shape[3]), weight_tensor.quantization.zero_point),
-                    ]
-                )
-            weight_tensor.values = padded_array
+        # Resize IFM
+        op.ifm_shapes[0] = Shape4D(
+            [ifm_shape.batch, ifm_shape.height, ifm_shape.width // resize_factor, ifm_shape.depth * resize_factor]
+        )
 
+        # Compute list of 0 padding for each dimensions of the filter
+        filter_dimension_padding = [(0, 0) for _ in weight_tensor.shape]
+        # Update padding for filter width with computed padding
+        filter_dimension_padding[1] = (left_filter_padding, right_filter_padding)
+        # Add padding to the filter
+        zero_point = weight_tensor.quantization.zero_point
+        padding_constant = zero_point if np.isscalar(zero_point) else 0
+        padded_filter_tensor = np.pad(weight_tensor.values, filter_dimension_padding, constant_values=padding_constant)
+        weight_shape[1] = padded_filter_tensor.shape[1]
+        weight_tensor.values = padded_filter_tensor
         # Change weight shape based on stride_x
-        weight_shape[1] //= stride_x
-        weight_shape[2] *= stride_x
+        weight_shape[1] //= resize_factor
+        weight_shape[2] *= resize_factor
 
         weight_tensor.values = np.reshape(weight_tensor.values, weight_shape)
         weight_tensor.set_all_shapes(weight_shape)
         # If multiple copies of the weights are used, we could avoid
         # them having the same address by changing the value_id
         weight_tensor.value_id = uuid.uuid4()
 
         # Strides
-        stride_x = 1
+        stride_x = final_stride
         op.attrs.update({"stride_w": stride_x, "stride_h": stride_y, "strides": (1, stride_y, stride_x, 1)})
 
     return op
 
 
 def convert_conv_to_fc(op, arch, nng):
     # Conv 1x1 can be equivalent to Fully Connected.
@@ -898,14 +1146,21 @@
             relu_fused_op.add_input_tensor(ifm)
             relu_fused_op.set_output_tensor(ofm)
             relu_fused_op.set_ifm_ofm_shapes()
             op = relu_fused_op
     return op
 
 
+def convert_lstm(op, arch, nng):
+    if op.type == Op.UnidirectionalSequenceLstm:
+        lstm = Lstm(op)
+        op = lstm.get_graph()
+    return op
+
+
 def convert_softmax(op, arch, nng):
     if op.type == Op.Softmax and op.run_on_npu:
         softmax = SoftMax(op)
         op = softmax.get_graph()
     return op
 
 
@@ -1358,19 +1613,14 @@
     if op.type == Op.Sigmoid:
         return convert_to_lut8(op, clamp_sigmoid, "sigmoid")
     elif op.type == Op.Tanh:
         return convert_to_lut8(op, math.tanh, "tanh")
     return op
 
 
-def remove_memory_only_ops(op, arch):
-    if op.run_on_npu and op.type in memory_only_ops:
-        bypass_memory_only_ops(op)
-
-
 def fuse_activation_function_with_prev(op, arch, nng):
     # if op is a no-op: attempts to move the activation function to the preceding op
     if not op.attrs.get("is_nop", False) or op.activation is None:
         return op
     ifm, ofm = op.get_ifm_ofm()
     if ifm is None or ofm is None:
         return op
@@ -1472,20 +1722,38 @@
                 quantization=quantization,
             )
             weight_tens.values = weights
             op.type = Op.DepthwiseConv2DBias
             op.inputs = []
             op.add_input_tensor(ifm)
             op.add_input_tensor(weight_tens)
-            # Add bias tensor, all biases set to 0
-            op.inputs.append(None)
-            fixup_bias_tensors(op, arch, nng, DataType.int32)
+
+            if op.ifm.dtype == DataType.uint8:
+                op.rounding_mode = RoundingMode.HalfUp
+
+                # Add bias tensor, all biases set to 0
+                op.inputs.append(None)
+                fixup_bias_tensors(op, arch, nng, DataType.int32)
+
+            else:
+                op.rounding_mode = RoundingMode.AwayZero
+
+                # The DepthwiseConv needs to be performed with the IFM zero point set appropriately so that the correct
+                # pad values are used. However, in order to use the rounding away from zero mode the zero point needs to
+                # have been removed so that the zero point is at zero. This is done by adding a kernel sized amount of
+                # the zero point as a bias. The datatype of the bias needs to be set to int32, even for an int16 IFM,
+                # because this will cause full precision scaling to be used (see weight compression). Finally, the OFM
+                # zero point will need forcing to zero (as it has already been removed)
+                nr_biases = op.inputs[1].shape[-1]
+                bias_values = [op.ifm.quantization.zero_point * k_h * k_w] * nr_biases
+                bias_tensor = create_const_tensor(op.name + "_bias", [nr_biases], DataType.int32, bias_values)
+                op.add_input_tensor(bias_tensor)
+
             # Add other inputs
             op.inputs.extend(other_inputs)
-            op.rounding_mode = NpuRoundingMode.NATURAL
 
         # Bypass the PAD operator
         op.set_input_tensor(pad_op.ifm, 0)
         # Adjust the padding attributes of the convolution operator
         op.attrs["padding"] = Padding.EXPLICIT
         op.attrs["explicit_padding"] = (top, left, bottom, right)
         op.set_ifm_ofm_shapes()
@@ -1615,35 +1883,31 @@
 def fixup_or_check_asymmetric_weights(force_symmetric_int_weights):
     if force_symmetric_int_weights:
         return fixup_asymmetric_weights
     else:
         return check_asymmetric_weights
 
 
-def convert_mean_to_depthwise_conv_or_avgpool(op, arch, nng):
+def convert_mean_to_depthwise_conv(op, arch, nng):
     if op.type == Op.Mean and op.run_on_npu:
         inp, axis = op.inputs
         shape = inp.shape
         ofm_shape = op.ofm.shape
         dims = len(shape)
         dims_ofm = len(ofm_shape)
 
         # Height and width axes have different index depending on dimensions
         if axis.shape == [] or axis.shape[0] == 1:  # single axis
             axis = int(axis.values) if len(axis.shape) == 0 else int(axis.values[0])
             if dims in (2, 3):
-                if axis == 0:
-                    h, w = shape[axis], 1
-                else:
-                    h, w = 1, shape[axis]
+                # If dims is 2 or 3, axis 0 refers to h-dimension
+                h, w = (shape[axis], 1) if axis == 0 else (1, shape[axis])
             else:
-                if axis == 1:
-                    h, w = shape[axis], 1
-                else:
-                    h, w = 1, shape[axis]
+                # If dims is 4, axis 1 refers to h-dimension
+                h, w = (shape[axis], 1) if axis == 1 else (1, shape[axis])
         else:  # multiple axes
             axis = sorted(axis.values)
             h, w = [shape[i] for i in axis]
 
         # Set necessary depthwise attributes
         op.attrs.update(
             {
@@ -1659,31 +1923,14 @@
             }
         )
         # Change op type
         op.type = Op.DepthwiseConv2DBias
         # Set IFM/OFM shapes after changing op type
         op.set_ifm_ofm_shapes()
 
-        weight_scale, bias = 1, 0
-        ofmq, ifmq = op.ofm.quantization, inp.quantization
-        if ifmq.is_scaling_equal(ofmq):
-            # Here we can just use a simple AvgPool with truncating rounding,
-            # as we're emulating simple integer division.
-            op.rounding_mode = NpuRoundingMode.TRUNCATE
-            op.type = Op.AvgPool
-            op.attrs.update({"ksize": (1, h, w, 1), "filter_height": h, "filter_width": w})
-        else:
-            op.rounding_mode = NpuRoundingMode.NATURAL
-            weight_scale = 1 / (h * w)
-            # Input zero point is adjusted after mean calculation, so we emulate that with a bias
-            bias = -ifmq.zero_point * h * w
-            fiq = ifmq.clone()
-            fiq.zero_point = 0
-            op.forced_input_quantization = fiq
-
         # Change dimensions to 4
         def extend_dims(dim, in_shape):
             if dim < 4:
                 in_shape = [1] + in_shape
                 if dim == 2:
                     in_shape += [1]
             return in_shape
@@ -1698,60 +1945,113 @@
                     ofm_shape.insert(i, 1)
             shape = extend_dims(dims, shape)
             dims_ofm = len(ofm_shape)
             ofm_shape = extend_dims(dims_ofm, ofm_shape)
             op.set_ifm_ofm_shapes()
 
         # If height is greater than max kernel height, reshape from HxW to 1x(HxW)
-        weight_shape = None
-        if (h > 64 and op.type == Op.DepthwiseConv2DBias) or (h > 256 and op.type == Op.AvgPool):
+        if h > 64:
             # This can only happen and be done for multiple axes, and
-            # h * w <= 256 for DepthwiseConv2DBias
-            # h * w <= 4096 for AvgPool
+            # h * w <= 4096 for DepthwiseConv2DBias
             # which is checked in supported ops
             shape = [shape[0], 1, h * w, shape[3]]
             op.ifm_shapes[0] = Shape4D(shape)
             weight_shape = [1, h * w, shape[3], shape[0]]
-            if h > 256 and op.type == Op.AvgPool:
-                op.attrs.update({"ksize": (1, 1, h * w, 1), "filter_height": 1, "filter_width": h * w})
-
-        # If the AvgPool version is used, we don't need to do anything else
-        if op.type == Op.AvgPool:
-            DebugDatabase.add_optimised(op, op)
-            return op
-
-        # Make unit weight tensor quantization
-        weight_quant = ifmq.clone()
-        weight_quant.min = 0
-        weight_quant.max = 255
-        weight_quant.scale_f32 = weight_scale
-        weight_quant.zero_point = 0
-
-        if weight_shape is None:
+        else:
             # Set weight shape to [H,W,C,B]
             weight_shape = [h, w, shape[3], shape[0]]
 
+        op.rounding_mode = RoundingMode.HalfUp
+        identity_quant = QuantizationParameters(scale_f32=1.0, zero_point=0)
+        op.forced_input_quantization = identity_quant
+        op.forced_output_quantization = identity_quant
+
         # Add unit weight tensor
         op.set_input_tensor(
             create_const_tensor(
                 "weights",
                 weight_shape,
                 inp.dtype,
                 np.ones(weight_shape),
-                quantization=weight_quant,
+                quantization=identity_quant,
             ),
             1,
         )
         op.weights.values = np.reshape(op.inputs[1].values, weight_shape)
 
-        # Add bias tensor
+        # Input zero point is adjusted after the sum calculation, so we emulate that with a bias
+        ofmq, ifmq = op.ofm.quantization, inp.quantization
+        bias = -ifmq.zero_point * h * w
         bias_shape = [shape[-1]]
-        op.inputs.append(create_const_tensor("bias", bias_shape, DataType.int32, np.ones(bias_shape) * bias))
+        op.inputs.append(create_const_tensor(op.name + "_bias", bias_shape, DataType.int32, np.ones(bias_shape) * bias))
         DebugDatabase.add_optimised(op, op)
 
+        # Create intermediate tensor between depthwise conv and mul
+        intermediate = op.ofm.clone(suffix="_intermediate", set_unique=True)
+        intermediate.dtype = DataType.int32
+
+        # Multiply sum with 1/num_elements_in_axis to get the mean
+        mul_op = Operation(Op.Mul, op.name + "_mul")
+        mul_op.add_input_tensor(intermediate)
+        mul_op.set_output_tensor(op.ofm)
+        mul_op.forced_input_quantization = identity_quant
+
+        # Set dw conv output to the intermediate tensor
+        op.set_output_tensor(intermediate)
+
+        # Move activation from original op to mean op
+        mul_op.activation = op.activation
+        op.activation = None
+
+        # The multiplier is calculated in the same way as in the reference,
+        # clamping the shift value at the price of some precision loss.
+        num_elements_in_axis = int(h * w)
+        output_multiplier, output_shift_vela = quantise_scale(np.double(ifmq.scale_f32) / np.double(ofmq.scale_f32))
+
+        # Convert to reference representation shift value
+        output_shift = 31 - output_shift_vela
+
+        # Reference calculation
+        # round_down_log2 same as 63 - CountLeadingZeros(num_elements_in_axis)
+        shift = round_down_log2(num_elements_in_axis)
+        shift = min(shift, 32)
+        shift = min(shift, 31 + output_shift)
+        output_multiplier = (output_multiplier << shift) // num_elements_in_axis
+        output_shift = output_shift - shift
+
+        # Convert to vela representation shift
+        output_shift_vela = 31 - output_shift
+
+        # For int32 scaling is not supported so instead multiply with the scale
+        # intermediate * scale -> round and shift.
+        scalar = create_const_tensor(
+            op.name + "_scalar", [1, 1, 1, 1], DataType.int32, [output_multiplier], quantization=identity_quant
+        )
+        mul_op.add_input_tensor(scalar)
+        mul_op.set_ifm_ofm_shapes()
+
+        # Reference using TFL rounding for the multiply
+        mul_op.rounding_mode = RoundingMode.TFLite
+
+        # Need to use explicit scaling to get the wanted shift
+        mul_op.explicit_scaling = ExplicitScaling(False, [output_shift_vela], [1])
+        DebugDatabase.add_optimised(op, mul_op)
+    return op
+
+
+def convert_ops_to_lut(op, arch, nng):
+    if op.type == Op.Exp:
+        if op.ifm.dtype == DataType.int8:
+            return create_lut_8bit_op(op, math.exp, "exp")
+        elif op.ifm.dtype == DataType.int16:
+            return create_lut_int16_op(op, math.exp, "exp")
+        else:
+            # Should already be catched in tflite supported ops
+            assert False, f"Unsupported data type {op.ifm.dtype} for {op.type}"
+
     return op
 
 
 def optimise_quantize(op: Operation, arch, nng):
 
     if op.type == Op.Quantize and op.run_on_npu:
 
@@ -1888,14 +2188,76 @@
             op.attrs["dilation"] = (1, hw_dilation_h, hw_dilation_w, 1)  # nhwc format
             op.attrs["dilation_h_factor"] = hw_dilation_h
             op.attrs["dilation_w_factor"] = hw_dilation_w
 
     return op
 
 
+def fixup_reshape(op, arch, nng):
+    def _get_explicit_shape(implicit_shape, total_size):
+        # the explicit shape is a copy of the implicit shape but with the special -1 (remaining size) value converted to
+        # the appropriate value
+        if implicit_shape is None:
+            return None
+
+        explicit_shape = list(implicit_shape)
+        if -1 in explicit_shape:
+            explicit_shape[explicit_shape.index(-1)] = int(total_size / abs(np.prod(implicit_shape)))
+
+        return explicit_shape
+
+    if op.type == Op.Reshape:
+        ifm_tensor, _, ofm_tensor = op.get_ifm_ifm2_ofm()
+        ifm_size = ifm_tensor.elements()
+        ofm_shape = ofm_tensor.shape
+
+        new_shape_tensor_shape = op.inputs[1].values.flatten() if len(op.inputs) > 1 else None
+        new_shape_tensor_shape = _get_explicit_shape(new_shape_tensor_shape, ifm_size)
+
+        new_shape_attribute = op.attrs.get("new_shape", None)
+        new_shape_attribute = _get_explicit_shape(new_shape_attribute, ifm_size)
+
+        # if present the new shape tensor overrides the new_shape attribute
+        if new_shape_tensor_shape is not None:
+            # check tensor
+            if not np.array_equal(new_shape_tensor_shape, ofm_shape):
+                print(
+                    f"Warning: {optype_to_builtintype(op.type)} '{op.name}' has new shape tensor"
+                    f" ({new_shape_tensor_shape}) that does not match output tensor shape {ofm_shape}. Will use output"
+                    f" tensor shape."
+                )
+        elif new_shape_attribute is not None:
+            # check attribute
+            if not np.array_equal(new_shape_attribute, ofm_shape):
+                print(
+                    f"Warning: {optype_to_builtintype(op.type)} '{op.name}' has new_shape attribute"
+                    f" ({new_shape_attribute}) that does not match output tensor shape {ofm_shape}. Will use output"
+                    f" tensor shape."
+                )
+        else:
+            print(
+                f"Warning: {optype_to_builtintype(op.type)} '{op.name}' does not have a new shape tensor or a new_shape"
+                f" attribute. Will use output tensor shape {ofm_shape}."
+            )
+
+        # force new shape tensor to output shape
+        new_shape_tensor = create_const_tensor(
+            op.name + "_new_shape", [len(ofm_shape)], DataType.int32, np.array(ofm_shape, np.int32)
+        )
+        if len(op.inputs) > 1:
+            op.set_input_tensor(new_shape_tensor, 1)
+        else:
+            op.add_input_tensor(new_shape_tensor)
+
+        # force new_shape attribute to output shape
+        op.attrs["new_shape"] = ofm_shape
+
+    return op
+
+
 def supported_operator_check(op, arch, nng):
     op.run_on_npu = arch.tflite_supported_operators.is_operator_supported(op)
     return op
 
 
 def tflite_optimise_graph(nng, arch, force_symmetric_int_weights):
     # Compile time static optimisations
@@ -1912,15 +2274,15 @@
             arch,
             [],
             optimisation_list,
             rewrite_unsupported=False,
         )
 
     # Pre-processing step
-    pre_process_list = [supported_operator_check, set_ifm_ofm_op_shapes]
+    pre_process_list = [supported_operator_check, set_ifm_ofm_op_shapes, fixup_reshape]
 
     for idx, sg in enumerate(nng.subgraphs):
         nng.subgraphs[idx] = rewrite_graph.rewrite_graph_pre_order(
             nng,
             sg,
             arch,
             [],
@@ -1950,47 +2312,45 @@
             sg,
             arch,
             [rewrite_split_ops],
             [],
             rewrite_unsupported=False,
         )
 
-    # Handle sg input output
+    # Bypass or rewrite memory only operators
     for idx, sg in enumerate(nng.subgraphs):
         nng.subgraphs[idx] = rewrite_graph.rewrite_graph_pre_order(
             nng,
             sg,
             arch,
             [],
-            [fix_sg_input_output],
+            [bypass_memory_only_ops],
             rewrite_unsupported=False,
         )
 
-    # Removal of memory only operators
-    for sg in nng.subgraphs:
-        rewrite_graph.visit_graph_post_order(sg.output_tensors, arch, [], [remove_memory_only_ops])
-        sg.refresh_after_modification()
-
     # Rewrite of operators
     op_rewrite_list = [
         set_tensor_equivalence,
-        convert_mean_to_depthwise_conv_or_avgpool,
+        convert_ops_to_lut,
+        convert_mean_to_depthwise_conv,
         convert_depthwise_to_conv,
         convert_conv_to_fc,
+        convert_lstm,
         convert_softmax,
         convert_prelu,
         convert_mul_max_to_abs_or_lrelu,
         convert_lrelu,
         fixup_strided_conv,
         convert_hardswish_to_lut,
         rewrite_fully_connected_input,
         convert_batched_fc_shape,
         fixup_conv2d_backprop,
         fixup_relus_with_differing_ifm_ofm_scaling,
         reorder_depthwise_weights,
+        convert_argmax_to_depthwise_conv_and_max_pool,
         fixup_resize,
         fixup_bias_tensors,
         fixup_asymmetric_weights,
         convert_tanh_sigmoid_to_lut,
         replace_pad_by_hw_pad,
         fixup_dilation_gt2,
     ]
```

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite_mapping.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite_mapping.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright 2020-2022 Arm Limited and/or its affiliates <open-source-office@arm.com>
+# SPDX-FileCopyrightText: Copyright 2020-2023 Arm Limited and/or its affiliates <open-source-office@arm.com>
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 # Licensed under the Apache License, Version 2.0 (the License); you may
 # not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -158,14 +158,15 @@
 
 
 def inverse_map(map):
     return {v: k for k, v in map.items()}
 
 
 datatype_map = {
+    TensorType.INT4: DataType.int4,
     TensorType.UINT8: DataType.uint8,
     TensorType.INT8: DataType.int8,
     TensorType.INT16: DataType.int16,
     TensorType.INT32: DataType.int32,
     TensorType.INT64: DataType.int64,
     TensorType.FLOAT16: DataType.float16,
     TensorType.FLOAT32: DataType.float32,
@@ -180,14 +181,15 @@
     TensorType.UINT32: DataType.uint32,
     TensorType.UINT16: DataType.uint16,
 }
 
 datatype_inv_map = inverse_map(datatype_map)
 datatype_inv_map[DataType.quint8] = TensorType.UINT8
 
+datatype_inv_map[DataType.qint4] = TensorType.INT4
 datatype_inv_map[DataType.qint8] = TensorType.INT8
 datatype_inv_map[DataType.qint16] = TensorType.INT16
 datatype_inv_map[DataType.qint32] = TensorType.INT32
 
 
 datatype_map_numpy = {
     TensorType.UINT8: np.uint8,
@@ -414,35 +416,43 @@
                 underscore_mem = mem
                 camelcase_mem = underscore_to_camel_case(mem)
                 self.members.append((underscore_mem, camelcase_mem, deserialize, serialize, is_vector))
 
     def deserialize(self, op_data):
         builtin_options = op_data.BuiltinOptions()
         attrs = {}
+        attrs["attribute_read_error"] = []  # list of attributes that couldn't be read, empty indicates no error
         if builtin_options:
             tfattrs = self.cls()
             tfattrs.Init(builtin_options.Bytes, builtin_options.Pos)
-            for underscore_mem, camelcase_mem, deserialize, serialize, is_vector in self.members:
+            for underscore_mem, camelcase_mem, deserialize, _, is_vector in self.members:
                 fun = camelcase_mem
                 if is_vector:
                     fun += "AsNumpy"
 
                 attr = getattr(tfattrs, fun)()
                 try:
                     attrs[underscore_mem] = deserialize(attr)
                 except TypeError:
-                    print("Warning: {0} could not read attribute '{1}'.".format(self.name, underscore_mem))
+                    attrs["attribute_read_error"].append(underscore_mem)
+        else:
+            # all builtin operators should have an options field
+            attrs["attribute_read_error"] = [underscore_mem for underscore_mem, *_ in self.members]
 
         return attrs
 
     def serialize(self, builder, attrs):
         ser_attrs = []
-        for underscore_mem, camelcase_mem, deserialize, serialize, is_vector in self.members:
-            a = serialize(builder, attrs[underscore_mem])
-            ser_attrs.append((camelcase_mem, a))
+        attrs["attribute_write_error"] = []  # list of attributes that couldn't be read, empty indicates no error
+        for underscore_mem, camelcase_mem, _, serialize, _ in self.members:
+            try:
+                a = serialize(builder, attrs[underscore_mem])
+                ser_attrs.append((camelcase_mem, a))
+            except KeyError:
+                attrs["attribute_write_error"].append(underscore_mem)
 
         getattr(self.module, self.name + "Start")(builder)
 
         for camelcase_mem, a in ser_attrs:
             getattr(self.module, self.name + "Add" + camelcase_mem)(builder, a)
 
         return getattr(self.module, self.name + "End")(builder), None
@@ -453,24 +463,28 @@
     CUSTOM_OPTIONS_FORMAT_DEFAULT = 0
 
     def __init__(self):
         self.custom_opt_format = 0
 
     def deserialize(self, op_data):
         attrs = {}
+        attrs["attribute_read_error"] = []  # list of attributes that couldn't be read, empty indicates no error
+
         custom_options = op_data.CustomOptionsAsNumpy()
         attrs["custom_options"] = custom_options
         attrs["custom_options_format"] = op_data.CustomOptionsFormat()
 
         if np.array_equal(custom_options, self.CUSTOM_OPTIONS_NPU_OP):
             attrs["custom_type"] = CustomType.ExistingNpuOp
 
         return attrs
 
     def serialize(self, builder, attrs):
+        attrs["attribute_write_error"] = []  # list of attributes that couldn't be written, empty indicates no error
+
         custom_type = attrs.get("custom_type", CustomType.ThirdPartyOp)
         self.custom_opt_format = attrs.get("custom_options_format", self.CUSTOM_OPTIONS_FORMAT_DEFAULT)
 
         # Set NPU op custom options for the TensorFlow Lite custom operator
         if custom_type == CustomType.NpuOp:
             custom_options = self.CUSTOM_OPTIONS_NPU_OP
         else:
@@ -716,15 +730,15 @@
     BuiltinOperator.BIDIRECTIONAL_SEQUENCE_RNN: (
         Op.BidirectionalSequenceRnn,
         OptionsSerializer(
             "BidirectionalSequenceRNNOptions", ("asymmetric_quantize_inputs", fused_act, "merge_outputs", "time_major")
         ),
         TFLITE_IFM_WEIGHTS_INDICES,
     ),
-    BuiltinOperator.EXP: (Op.Exp, OptionsSerializer("ExpOptions"), TFLITE_NO_INDICES),
+    BuiltinOperator.EXP: (Op.Exp, OptionsSerializer("ExpOptions"), TFLITE_IFM_INDICES),
     BuiltinOperator.TOPK_V2: (Op.TopKV2, OptionsSerializer("TopKV2Options"), TFLITE_NO_INDICES),
     BuiltinOperator.SPLIT: (Op.Split, OptionsSerializer("SplitOptions", ("num_splits",)), TFLITE_SPLIT_IFM_INDICES),
     BuiltinOperator.LOG_SOFTMAX: (Op.LogSoftmax, OptionsSerializer("LogSoftmaxOptions"), TFLITE_NO_INDICES),
     BuiltinOperator.DELEGATE: (Op.Delegate, None, TFLITE_NO_INDICES),
     BuiltinOperator.BIDIRECTIONAL_SEQUENCE_LSTM: (
         Op.BidirectionalSequenceLstm,
         OptionsSerializer(
@@ -745,15 +759,15 @@
         TFLITE_NO_INDICES,
     ),
     BuiltinOperator.PRELU: (Op.Prelu, None, TFLITE_IFM_IFM2_INDICES),
     BuiltinOperator.MAXIMUM: (Op.Maximum, OptionsSerializer("MaximumMinimumOptions"), TFLITE_IFM_IFM2_INDICES),
     BuiltinOperator.ARG_MAX: (
         Op.ArgMax,
         OptionsSerializer("ArgMaxOptions", (("output_type", datatype_deserialize, datatype_serialize),)),
-        TFLITE_NO_INDICES,
+        TFLITE_IFM_INDICES,
     ),
     BuiltinOperator.MINIMUM: (Op.Minimum, OptionsSerializer("MaximumMinimumOptions"), TFLITE_IFM_IFM2_INDICES),
     BuiltinOperator.LESS: (Op.Less, OptionsSerializer("LessOptions"), TFLITE_NO_INDICES),
     BuiltinOperator.NEG: (Op.Neg, OptionsSerializer("NegOptions"), TFLITE_NO_INDICES),
     BuiltinOperator.PADV2: (Op.PadV2, OptionsSerializer("PadV2Options"), TFLITE_NO_INDICES),
     BuiltinOperator.GREATER: (Op.Greater, OptionsSerializer("GreaterOptions"), TFLITE_NO_INDICES),
     BuiltinOperator.GREATER_EQUAL: (Op.GreaterEqual, OptionsSerializer("GreaterEqualOptions"), TFLITE_NO_INDICES),
```

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite_model_semantic.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite_model_semantic.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from .data_type import BaseType
 from .data_type import DataType
 from .numeric_util import is_integer
 from .operation import Op
 from .supported_operators_util import docstring_format_args
 from .supported_operators_util import list_formatter
 from .tensor import check_quantized_tens_scaling_equal
+from .tensor import shape_num_elements
 from .tflite_mapping import BUILTIN_OPERATOR_UNKNOWN
 from .tflite_mapping import optype_to_builtintype
 
 
 def _optype_formatter(op_list):
     # Convert internal op types to external names
     output = map(optype_to_builtintype, op_list)
@@ -72,27 +73,30 @@
             Op.Add,
             Op.Mul,
             Op.Sub,
         )
     )
     binary_elem_wise_main_ops = binary_elem_wise_min_max_ops | binary_elem_wise_add_mul_sub | binary_elem_wise_shift_ops
     elem_wise_main_ops = binary_elem_wise_main_ops | unary_elem_wise_main_ops
-    shapeless_input_ops = binary_elem_wise_main_ops | set((Op.Split, Op.SplitV, Op.Mean, Op.ExpandDims, Op.Quantize))
+    shapeless_input_ops = binary_elem_wise_main_ops | set(
+        (Op.Split, Op.SplitV, Op.Mean, Op.ExpandDims, Op.Quantize, Op.ArgMax)
+    )
     reshape_ops = set(
         (
             Op.Reshape,
             Op.QuantizedReshape,
             Op.Squeeze,
             Op.ExpandDims,
         )
     )
 
     def __init__(self):
         # Setup the generic constraints. Note: the order matters
         self.generic_constraints = []
+        self.generic_constraints.append(TFLiteSemantic.constraint_attributes_specified)
         self.generic_constraints.append(TFLiteSemantic.constraint_tens_no_dynamic)
         self.generic_constraints.append(TFLiteSemantic.constraint_tens_defined_shape)
         self.generic_constraints.append(TFLiteSemantic.constraint_tens_output_scalar)
         self.generic_constraints.append(TFLiteSemantic.constraint_tens_input_scalar)
         self.generic_constraints.append(TFLiteSemantic.constraint_tens_shape_size)
 
         self.generic_constraints.append(TFLiteSemantic.constraint_tens_quant_none_check)
@@ -144,14 +148,15 @@
             self.specific_constraints[op_type].append(TFLiteSemantic.constraint_matching_inputs_types)
             self.specific_constraints[op_type].append(TFLiteSemantic.constraint_matching_signed)
             self.specific_constraints[op_type].append(TFLiteSemantic.constraint_unsigned_valid)
 
         # Ops reshaping dimensions: Reshape, Squeeze and ExpandDims
         for op_type in TFLiteSemantic.reshape_ops:
             self.specific_constraints[op_type].append(TFLiteSemantic.constraint_matching_in_out_quant)
+            self.specific_constraints[op_type].append(TFLiteSemantic.constraint_matching_in_out_elements)
 
         # Softmax specific checks:
         self.specific_constraints[Op.Softmax].append(TFLiteSemantic.constraint_matching_shapes)
         self.specific_constraints[Op.Softmax].append(TFLiteSemantic.constraint_matching_in_out_types)
         self.specific_constraints[Op.Softmax].append(TFLiteSemantic.constraint_beta_value_range)
 
         # Split specific checks:
@@ -177,18 +182,32 @@
         self.specific_constraints[Op.Pad].append(TFLiteSemantic.constraint_pad_constant)
 
         # HardSwish specific checks:
         self.specific_constraints[Op.HardSwish].append(TFLiteSemantic.constraint_input_8bit)
         self.specific_constraints[Op.HardSwish].append(TFLiteSemantic.constraint_matching_in_out_types)
 
         # Mean specific checks:
-        self.specific_constraints[Op.Mean].append(TFLiteSemantic.constraint_input_8bit)
         self.specific_constraints[Op.Mean].append(TFLiteSemantic.constraint_mean_input_dims)
         self.specific_constraints[Op.Mean].append(TFLiteSemantic.constraint_mean_axis)
 
+        # ArgMax specific checks:
+        self.specific_constraints[Op.ArgMax].append(TFLiteSemantic.constraint_input_8bit)
+        self.specific_constraints[Op.ArgMax].append(TFLiteSemantic.constraint_argmax_output)
+
+        # UnidirectionalSequenceLstm specific checks:
+        self.specific_constraints[Op.UnidirectionalSequenceLstm].append(TFLiteSemantic.constraint_input_signed)
+        self.specific_constraints[Op.UnidirectionalSequenceLstm].append(TFLiteSemantic.constraint_matching_in_out_types)
+        self.specific_constraints[Op.UnidirectionalSequenceLstm].append(TFLiteSemantic.constraint_lstm_dimensions)
+        self.specific_constraints[Op.UnidirectionalSequenceLstm].append(TFLiteSemantic.constraint_lstm_inputs)
+        self.specific_constraints[Op.UnidirectionalSequenceLstm].append(TFLiteSemantic.constraint_lstm_intermediates)
+        self.specific_constraints[Op.UnidirectionalSequenceLstm].append(TFLiteSemantic.constraint_lstm_variables)
+
+        # Exp specific checks
+        self.specific_constraints[Op.Exp].append(TFLiteSemantic.constraint_input_signed)
+
     def is_operator_semantic_valid(self, op):
         ext_type = optype_to_builtintype(op.type)
 
         if op.type in (Op.Placeholder, Op.SubgraphInput, Op.Const):
             return True
 
         # Generic constraints list filtered out to exclude certain constraints depending on op.type
@@ -220,14 +239,17 @@
             Op.Shape: [
                 TFLiteSemantic.constraint_tens_quant_none_check,
             ],
             Op.Quantize: [
                 TFLiteSemantic.constraint_tens_no_dynamic,
                 TFLiteSemantic.constraint_tens_output_scalar,
             ],
+            Op.ArgMax: [
+                TFLiteSemantic.constraint_tens_quant_none_check,
+            ],
         }
         return generic_constraints_exclude_list
 
     @staticmethod
     def constraint_none_const_tensors(op):
         "Constant tensors should not have NoneType-values"
         valid = True
@@ -235,14 +257,24 @@
         for tens in filter(None, op.inputs):
             if len(tens.ops) > 0 and tens.ops[0].type == Op.Const and tens.values is None:
                 valid = False
                 extra = str(tens.name)
         return valid, f"Unexpected None value for constant tensor: {extra}"
 
     @staticmethod
+    def constraint_attributes_specified(op):
+        "All required operator attributes must be specified"
+        # operators that have been created internally (i.e. not created as part of reading an input network) may not
+        # have the read error attribute
+        attribute_read_error = op.attrs.get("attribute_read_error", [])
+        valid = len(attribute_read_error) == 0
+        extra = ", ".join(attribute_read_error)
+        return valid, f"Op has missing attributes: {extra}"
+
+    @staticmethod
     def constraint_tens_no_dynamic(op):
         "Input(s) and Output tensors must not be dynamic"
         valid = True
         extra = []
         tensors = [tens for tens in op.inputs + op.outputs if tens]
         for tens in tensors:
             if (tens.shape == []) and (tens.values is None):
@@ -613,21 +645,35 @@
         ifm_dtype = op.ifm.dtype
         ofm_dtype = op.ofm.dtype
         if ifm_dtype.type & BaseType.Unsigned:
             valid = (ifm_dtype == ofm_dtype) or (ofm_dtype == DataType.int32)
         return valid, f"Op has ifm_dtype={ifm_dtype} and ofm_dtype={ofm_dtype}"
 
     @staticmethod
+    def constraint_input_signed(op):
+        "IFM must be int8 or int16"
+        ifm_dtype = op.ifm.dtype
+        valid = (ifm_dtype == DataType.int8) or (ifm_dtype == DataType.int16)
+        return valid, f"Op has ifm_dtype={ifm_dtype}"
+
+    @staticmethod
     def constraint_input_8bit(op):
         "IFM must be int8 or uint8"
         ifm_dtype = op.ifm.dtype
         valid = (ifm_dtype == DataType.int8) or (ifm_dtype == DataType.uint8)
         return valid, f"Op has ifm_dtype={ifm_dtype}"
 
     @staticmethod
+    def constraint_argmax_output(op):
+        "OFM must be int32 or int64"
+        ofm_dtype = op.ofm.dtype
+        valid = ofm_dtype in (DataType.int32, DataType.int64)
+        return valid, f"Op has ofm_dtype={ofm_dtype}"
+
+    @staticmethod
     def constraint_matching_either_shapes(op):
         "At least one Input's shape must match the OFM's shape"
         ifm_shape = op.ifm.shape
         ifm2_shape = op.ifm2.shape if op.ifm2 else None
         ofm_shape = op.ofm.shape
         valid = (ifm_shape == ofm_shape) or (ifm2_shape == ofm_shape)
         return valid, f"Op has ifm_shape={ifm_shape}, ifm2_shape={ifm2_shape} and ofm_shape={ofm_shape}"
@@ -660,14 +706,51 @@
     @staticmethod
     def constraint_matching_in_out_quant(op):
         "Input and output quantisation must match."
         if not check_quantized_tens_scaling_equal(op.ifm, op.ofm):
             return False, "IFM and OFM quantisation parameters are not equal."
         return True, "IFM and OFM quantisation parameters matches."
 
+    @staticmethod
+    def constraint_matching_in_out_elements(op):
+        "Input and output number of elements must match."
+        if shape_num_elements(op.ifm.shape) != shape_num_elements(op.ofm.shape):
+            return False, f"IFM {op.ifm.shape} and OFM {op.ofm.shape} number of elements are not equal."
+        return True, "IFM and OFM number of elements are equal."
+
+    @staticmethod
+    def constraint_lstm_dimensions(op):
+        "IFM and OFM must have 3D shape"
+        valid = len(op.ifm.shape) == len(op.ofm.shape) == 3
+        return valid, f"Op has ifm shape {op.ifm.shape} and ofm shape {op.ofm.shape}"
+
+    @staticmethod
+    def constraint_lstm_inputs(op):
+        "Must have 24 input tensors"
+        n_inputs = len(op.inputs)
+        return n_inputs == 24, f"Op has {n_inputs} inputs"
+
+    @staticmethod
+    def constraint_lstm_intermediates(op):
+        "Must have 5 intermediate tensors"
+        n_intermediates = len(op.intermediates)
+        return n_intermediates == 5, f"Op has {n_intermediates} intermediates"
+
+    @staticmethod
+    def constraint_lstm_variables(op):
+        "State tensors must be variable"
+        valid = True
+        extra = []
+        for tens in op.inputs[18:20]:
+            if not tens.is_variable:
+                valid = False
+                extra.append(tens.name)
+        extra = ", ".join(extra)
+        return valid, f"Op has non-variable state tensor(s): {extra}"
+
 
 def tflite_semantic_checker(nng):
     semantic_checker = TFLiteSemantic()
     for sg in nng.subgraphs:
         for op in sg.get_all_ops():
             op.run_on_npu = semantic_checker.is_operator_semantic_valid(op)
     return nng
```

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite_reader.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite_reader.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 from .tensor import Tensor
 from .tflite.BuiltinOperator import BuiltinOperator
 from .tflite.Model import Model
 from .tflite_mapping import builtin_operator_map
 from .tflite_mapping import DataType
 from .tflite_mapping import datatype_map
 from .tflite_mapping import datatype_map_numpy
+from .tflite_mapping import optype_to_builtintype
 
 
 class TFLiteSubgraph:
     def __init__(self, graph, subgraph):
         self.graph = graph
         self.name = decode_str(subgraph.Name())
 
@@ -112,27 +113,28 @@
             if dtype == DataType.string:
                 tens.values = np.array(buf.view(np_dtype))
             else:
                 tens.values = np.array(buf.view(np_dtype).reshape(shape))
         return tens
 
     def parse_operator(self, op_index, op_data):
-        op_type, opt_serializer, custom_code, indices = self.graph.operator_codes[op_data.OpcodeIndex()]
+        op_type, opt_serializer, custom_code, indices, version = self.graph.operator_codes[op_data.OpcodeIndex()]
         inputs = [self.tensors[idx] if idx != -1 else None for idx in op_data.InputsAsNumpy()]
         outputs = [self.tensors[idx] if idx != -1 else None for idx in op_data.OutputsAsNumpy()]
         intermediates = []
         if op_data.IntermediatesLength():
             intermediates = [self.tensors[idx] if idx != -1 else None for idx in op_data.IntermediatesAsNumpy()]
 
         name = "unknown_op_name"
         if len(outputs):
             name = outputs[0].name
         inputs = align_tensor_indices_to_nng(op_type, indices, inputs)
         op = Operation(op_type, name)
         op.op_index = op_index
+        op.version = version
         op.inputs = inputs
         op.outputs = outputs
         op.intermediates = intermediates
         for out in op.outputs:
             out.ops = [op]
 
         if op_type in (Op.AssignVariable, Op.CallOnce):
@@ -176,17 +178,19 @@
                     self.graph.nng.subgraphs[body_subgraph_index],
                 )
             if op_type == Op.CallOnce:
                 # Attach the actual nng subgraphs to the op
                 init_subgraph_index = op.attrs["init_subgraph_index"]
                 op.attrs["subgraph"] = (self.graph.nng.subgraphs[init_subgraph_index],)
 
-            if op_type == Op.Reshape and "new_shape" not in op.attrs:
-                # Reshape should have an attrib "new_shape" but if it is missing, add it based on the output shape
-                op.attrs["new_shape"] = outputs[0].shape
+            if op_type == Op.Reshape:
+                if "new_shape" in op.attrs["attribute_read_error"] and len(inputs) > 1:
+                    # the "new_shape" attribute is optional if the new_shape tensor (inputs[1]) is specified. therefore,
+                    # remove the attribute read error
+                    op.attrs["attribute_read_error"].remove("new_shape")
 
             if op_type == Op.Cast:
                 # Cast op should have "in/out_data_type" attribs add if missing
                 if "in_data_type" not in op.attrs:
                     op.attrs["in_data_type"] = inputs[0].dtype
                 if "out_data_type" not in op.attrs:
                     op.attrs["out_data_type"] = outputs[0].dtype
@@ -202,20 +206,33 @@
 
             if op_type == Op.DepthwiseConv2DBias and op.attrs["depth_multiplier"] == 0:
                 # The depth multiplier is implicit and is calculated as weight channels / ifm channels
                 # Note however that the weights have been reshaped above.
                 # The original value is cached above in channel_multiplier
                 op.attrs["depth_multiplier"] = op.weights.shape[2] // op.ifm.shape[-1]
 
-            faf = op.attrs.pop("fused_activation_function", None)
+            # The fused_activation_function attribute needs to be retained so that the
+            # tflite_writer can correctly pass through operators that run on the CPU.
+            # This is because the operator activation attribute is later converted to an
+            # NpuActivation which treats None and ReLU the same, thereby making it difficult
+            # for the tflite_writer to recover the original activation function.
+            faf = op.attrs.get("fused_activation_function", None)
             if faf is not None:
                 op.activation = create_activation_function(faf)
             if custom_code is not None:
                 op.attrs["custom_code"] = custom_code
 
+            # finally, report any missing attributes that could not be read during deserialize()
+            attribute_read_error = op.attrs["attribute_read_error"]
+            if len(attribute_read_error) != 0:
+                print(
+                    f"Warning: Could not read the following attributes from {optype_to_builtintype(op.type)}"
+                    f" '{op.name}' {opt_serializer.name} field: {', '.join(attribute_read_error)}"
+                )
+
     @staticmethod
     def len1_array_to_scalar(arr):
         # The following flatbuffer quantisation fields all return a scalar value of 0 if they are not definied in
         # the input buffer. This is represented in Vela by using None.
         # Otherwise, the fields returned are a single or multi-element array. In which case, single element arrays
         # are converted to scalars
         if isinstance(arr, int) and arr == 0:
@@ -240,17 +257,31 @@
 
         try:
             parsing_step = "parsing root"
             model = Model.GetRootAsModel(buf, 0)
 
             parsing_step = "parsing buffers length"
             self.buffers = []
-            for idx in range(model.BuffersLength()):
-                parsing_step = f"parsing buffer {idx}"
-                self.buffers.append(self.parse_buffer(model.Buffers(idx)))
+            if not model.BuffersIsNone():
+                for idx in range(model.BuffersLength()):
+                    parsing_step = f"parsing buffer {idx}"
+                    buffer = model.Buffers(idx)
+                    buffer_data = self.parse_buffer(buffer)
+                    # buffers can be either; empty, or contain no data (zero length), or contain data (non-zero length).
+                    # when a buffer is None it means that it is either empty or zero length, and an empty buffer
+                    # will have DataIsNone() equal to true.
+                    # we should detect zero length buffers and report a warning because the TFLite semantics for these
+                    # types of buffers changed in TensorFlow 2.11, whereby they could result in runtime errors
+                    if buffer_data is None and not buffer.DataIsNone():
+                        print(
+                            f"Warning: Input TensorFlow Lite network contains a zero length buffer (index = {idx})"
+                            f" which is semantically not empty. However, it will be treated as an empty buffer."
+                        )
+
+                    self.buffers.append(buffer_data)
 
             parsing_step = "parsing operator codes length"
             self.operator_codes = []
             for idx in range(model.OperatorCodesLength()):
                 parsing_step = f"parsing operator code {idx}"
                 self.operator_codes.append(self.parse_operator_code(model.OperatorCodes(idx)))
 
@@ -304,15 +335,15 @@
             raise InputFileError(
                 self.name, f"The input file contains operator code '{c}' which is currently not supported"
             )
         op_type, ser, indices = builtin_operator_map[c]
         custom_code = None
         if c == BuiltinOperator.CUSTOM:
             custom_code = decode_str(code.CustomCode())
-        return op_type, ser, custom_code, indices
+        return op_type, ser, custom_code, indices, code.Version()
 
 
 def read_tflite(filename, batch_size, feed_dict, output_node_names, initialisation_nodes):
     tflite_graph = TFLiteGraph(filename, batch_size, feed_dict, output_node_names, initialisation_nodes)
     nng = tflite_graph.nng
     nng.refresh_after_modification()
     return nng
```

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite_supported_operators.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite_supported_operators.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,26 +65,28 @@
         (
             Op.QuantizedMatMul,
             Op.MatMul,
             Op.FullyConnected,
         )
     )
     mac_main_ops = (
-        # RNN/LSTM/GRU
-        set((Op.BlockLSTM,))
+        # LSTM
+        set((Op.UnidirectionalSequenceLstm,))
         # conv/depthwiseconv/transposeconv
         | convolution_like_ops
         # pooling
         | pooling_ops
         # resizing/upscaling
         | resizing_ops
         # FC layers
         | fc_vector_products
         # Mean (converts to depthwise conv)
         | set((Op.Mean,))
+        # ArgMax (converts to depthwise conv and maxpool)
+        | set((Op.ArgMax,))
     )
     unary_elem_wise_main_ops = Op.op_set(Op.is_unary_elementwise_op)
     binary_elem_wise_min_max_ops = set(
         (
             Op.Minimum,
             Op.Maximum,
         )
@@ -102,23 +104,15 @@
             Op.Sub,
         )
     )
     binary_elem_wise_main_ops = binary_elem_wise_min_max_ops | binary_elem_wise_add_mul_sub | binary_elem_wise_shift_ops
     elem_wise_main_ops = binary_elem_wise_main_ops | unary_elem_wise_main_ops
     pad_ops = set((Op.Pad,))
     supported_int32_tensor_ops = (
-        set(
-            (
-                Op.ReduceSum,
-                Op.CLZ,
-                Op.Shape,
-            )
-        )
-        | binary_elem_wise_add_mul_sub
-        | binary_elem_wise_shift_ops
+        set((Op.ReduceSum, Op.CLZ, Op.Shape, Op.ArgMax)) | binary_elem_wise_add_mul_sub | binary_elem_wise_shift_ops
     )
 
     relu_ops = set(
         (
             Op.Relu,
             Op.Relu6,
             Op.ReluN1To1,
@@ -193,29 +187,29 @@
     dilated_height_range = (1, 64)
     dilated_product_range = (1, 64 * 64)
     weights_limit = 127 * 65536
     filter_range = (1, 8)
     filter_height_range = (1, 256)
     filter_product_range = (1, 256 * 256)
     mean_kernel_product = 64 * 64
-    mean_kernel_product_avgpool = 256 * 256
 
     def __init__(self):
         # Setup the generic constraints. Note: the order matters
         self.generic_constraints = []
         self.generic_constraints.append(TFLiteSupportedOperators.constraint_tens_dtype)
         self.generic_constraints.append(TFLiteSupportedOperators.constraint_tens_int32_ops)
         self.generic_constraints.append(TFLiteSupportedOperators.constraint_tens_dimension)
         self.generic_constraints.append(TFLiteSupportedOperators.constraint_tens_quant_per_axis)
         self.generic_constraints.append(TFLiteSupportedOperators.constraint_batch_size)
         self.generic_constraints.append(TFLiteSupportedOperators.constraint_faf)
         self.generic_constraints.append(TFLiteSupportedOperators.constraint_faf_type)
 
         # Setup generic constraint exceptions
         self.generic_constraints_exceptions = defaultdict(list)
+        self.generic_constraints_exceptions[Op.ArgMax].append(TFLiteSupportedOperators.constraint_tens_dtype)
         self.generic_constraints_exceptions[Op.FullyConnected].append(TFLiteSupportedOperators.constraint_batch_size)
         self.generic_constraints_exceptions[Op.Softmax].append(TFLiteSupportedOperators.constraint_batch_size)
         self.generic_constraints_exceptions[Op.Reshape].append(TFLiteSupportedOperators.constraint_batch_size)
         self.generic_constraints_exceptions[Op.Shape].append(TFLiteSupportedOperators.constraint_batch_size)
         self.generic_constraints_exceptions[Op.Squeeze].append(TFLiteSupportedOperators.constraint_batch_size)
         for op_type in TFLiteSupportedOperators.split_ops - set((Op.UnpackReshaped,)):
             self.generic_constraints_exceptions[op_type].append(TFLiteSupportedOperators.constraint_batch_size)
@@ -310,21 +304,32 @@
 
         # Pad specific checks:
         self.specific_constraints[Op.Pad].append(TFLiteSupportedOperators.constraint_pad_shape)
         self.specific_constraints[Op.Pad].append(TFLiteSupportedOperators.constraint_padding_dimensions)
         self.specific_constraints[Op.Pad].append(TFLiteSupportedOperators.constraint_pad_type)
 
         # Mean specific checks:
-        self.specific_constraints[Op.Mean].append(TFLiteSupportedOperators.constraint_mean_height_width_product_avgpool)
         self.specific_constraints[Op.Mean].append(TFLiteSupportedOperators.constraint_mean_height_width_product)
         self.specific_constraints[Op.Mean].append(TFLiteSupportedOperators.constraint_mean_height_single_axis)
 
         # Reshape specific checks:
         self.specific_constraints[Op.Reshape].append(TFLiteSupportedOperators.constraint_reshape_shape_constant)
 
+        # ArgMax specific checks:
+        self.specific_constraints[Op.ArgMax].append(TFLiteSupportedOperators.constraint_argmax_axis)
+        self.specific_constraints[Op.ArgMax].append(TFLiteSupportedOperators.constraint_argmax_depth)
+
+        # UnidirectionalSequenceLstm specific checks:
+        op_type = Op.UnidirectionalSequenceLstm
+        self.specific_constraints[op_type].append(TFLiteSupportedOperators.constraint_lstm_no_cifg)
+        self.specific_constraints[op_type].append(TFLiteSupportedOperators.constraint_lstm_no_peep_hole)
+        self.specific_constraints[op_type].append(TFLiteSupportedOperators.constraint_lstm_no_projection)
+        self.specific_constraints[op_type].append(TFLiteSupportedOperators.constraint_lstm_no_normalisation)
+        self.specific_constraints[op_type].append(TFLiteSupportedOperators.constraint_lstm_weights)
+
     def is_operator_supported(self, op):
         ext_type = optype_to_builtintype(op.type)
         if op.type not in TFLiteSupportedOperators.supported_operators:
             if op.type not in (Op.Placeholder, Op.SubgraphInput, Op.Const):
                 print(f"Info: {ext_type} '{op.name}' is a CPU only op")
             return False
 
@@ -533,20 +538,19 @@
                 f" and depth_multiplier={depth_multiplier}"
             )
             return valid, extra
         return True, "Op has depth_multiplier=1"
 
     @staticmethod
     def constraint_conv_stride(op):
-        "Stride values for height must be between 1 and 3 and for width between 1 and 4"
+        "Stride width must be greater than or equal to 1 and stride height must be between 1 and 3"
         w, h = op.get_kernel_stride()
-        stride_min_w_h = 1
-        stride_max_w = 4
+        stride_min = 1
         stride_max_h = 3
-        valid = (stride_min_w_h <= w <= stride_max_w) and (stride_min_w_h <= h <= stride_max_h)
+        valid = (stride_min <= w) and (stride_min <= h <= stride_max_h)
         return valid, f"Op has stride WxH as: {w}x{h}"
 
     @staticmethod
     def constraint_depthwise_conv_stride(op):
         "Stride values for both width and height must be between 1 and 3"
         w, h = op.get_kernel_stride()
         stride_min, stride_max = 1, 3
@@ -700,22 +704,27 @@
 
         if align_corners and half_pixel_centers:
             valid = False
         return valid, "Op has both align_corners and half_pixel_centers set to True."
 
     @staticmethod
     def constraint_resizebi_half_pixel_centers_dims(op):
-        """Half_pixel_centers for resize bilinear requires that OFM W and H is 2x IFM W and H"""
+        """For half_pixel_centers the width and height of the IFM and OFM must match one of the following criteria:
+        IFM W and H are both 1
+        OFM W and H is 2x IFM W and H"""
         half_pixel_centers = op.attrs.get("half_pixel_centers", False)
         if not half_pixel_centers:
             valid = True
         elif len(op.ifm.shape) >= 3:
             ifm_h, ifm_w = op.ifm.shape[-3:-1]
             ofm_h, ofm_w = op.ofm.shape[-3:-1]
-            valid = ofm_h / ifm_h == 2 and ofm_w / ifm_w == 2
+            if ifm_h == 1 and ifm_w == 1:
+                valid = True
+            else:
+                valid = ofm_h / ifm_h == 2 and ofm_w / ifm_w == 2
         else:
             # Unexpected IFM shape
             valid = False
         return (
             valid,
             f"Op has ifm_shape={op.ifm.shape}, ofm_shape={op.ofm.shape} and half_pixel_centers={half_pixel_centers}",
         )
@@ -798,46 +807,28 @@
                 if not (i == i2 or i == 1 or i2 == 1) or o != mi:
                     valid = False
                     break
 
         return valid, f"Op has ifm_shape={ifm_shape} and ifm2_shape={ifm2_shape}"
 
     @classmethod
-    @docstring_format_args([mean_kernel_product_avgpool])
-    def constraint_mean_height_width_product_avgpool(cls, op):
-        """Product of height and width must be no greater than {}"""
-        shape = op.inputs[0].shape
-        hi = 0 if len(shape) < 4 else 1
-        h, w = shape[hi : hi + 2]
-        max_prod = cls.mean_kernel_product_avgpool
-        return h * w <= max_prod, f"Product of height and width is {h * w}"
-
-    @classmethod
     @docstring_format_args([mean_kernel_product])
     def constraint_mean_height_width_product(cls, op):
-        """Product of height and width must be no greater than {} when:
-        IFM and OFM have different scale or zero point; or
-        'keep_dims' is True"""
-        ifmq, ofmq = op.ifm.quantization, op.ofm.quantization
-        keep_dims = op.attrs.get("keep_dims")
-        # doesn't apply, size is checked by constraint_mean_height_width_product_avgpool
-        if not keep_dims and ifmq.scale_f32 == ofmq.scale_f32 and ifmq.zero_point == ofmq.zero_point:
-            return True, ""
+        """Product of height and width must be no greater than {}"""
         shape = op.inputs[0].shape
         hi = 0 if len(shape) < 4 else 1
         h, w = shape[hi : hi + 2]
         max_prod = cls.mean_kernel_product
         return h * w <= max_prod, f"Product of height and width is {h * w}"
 
     @classmethod
-    @docstring_format_args([filter_height_range[1], dilated_height_range[1]])
+    @docstring_format_args([dilated_height_range[1]])
     def constraint_mean_height_single_axis(cls, op):
         """For single axis averages across the height dimension:
-        IFM height must be no greater than {} if the IFM and OFM scale and zero point match; otherwise
-        IFM height must be no greater than {} if the IFM and OFM scale or zero point do not match"""
+        IFM height must be no greater than {}"""
         inp, axis = op.inputs
         if axis.shape == [] or axis.shape[0] == 1:  # single axis
             axis = int(axis.values) if len(axis.shape) == 0 else int(axis.values[0])
         else:
             # Multiple axes
             return True, ""
 
@@ -848,28 +839,75 @@
         if axis != len(shape) - 3:
             # Not averaging across the height dimension
             return True, ""
 
         h = shape[axis]
         ifm, ofm = op.get_ifm_ofm()
 
-        if check_quantized_tens_scaling_equal(ifm, ofm):
-            return h <= cls.filter_height_range[1], f"Height is {h}, IFM and OFM quantizations match"
-        else:
-            return h <= cls.dilated_height_range[1], f"Height is {h}, IFM and OFM quantizations do not match"
+        return h <= cls.dilated_height_range[1], f"Height is {h}"
 
     @staticmethod
     def constraint_reshape_shape_constant(op):
         "Shape must be constant"
         valid = True
         extra = []
 
-        reshape_tens = op.inputs[1]
-        if reshape_tens is not None:
-            # constant inputs have either no driving operator or a const one
-            # create a list of non-constant inputs
-            if not (len(reshape_tens.ops) == 0 or reshape_tens.ops[0].type == Op.Const):
-                valid = False
-                extra.append(reshape_tens.name)
+        # if a reshape tensor is specified then it must be constant
+        if len(op.inputs) > 1:
+            reshape_tens = op.inputs[1]
+            if reshape_tens is not None:
+                # constant inputs have either no driving operator or a const one
+                # create a list of non-constant inputs
+                if not (len(reshape_tens.ops) == 0 or reshape_tens.ops[0].type == Op.Const):
+                    valid = False
+                    extra.append(reshape_tens.name)
         extra = ", ".join(extra)
 
         return valid, f"Op has non-const input(s): {extra}"
+
+    @staticmethod
+    def constraint_argmax_axis(op):
+        "Operation must be performed along the depth axis"
+        inp_dims = len(op.inputs[0].shape)
+        axis = op.inputs[1].values
+        return (
+            axis in (inp_dims - 1, -1),
+            f"Axis is {axis} and number of input dimensions is {inp_dims}",
+        )
+
+    @staticmethod
+    def constraint_argmax_depth(op):
+        "IFM depth must be no greater than 127"
+        ifm_depth = op.inputs[0].shape[-1]
+        return ifm_depth <= 127, f"IFM depth is {ifm_depth}"
+
+    @staticmethod
+    def constraint_lstm_no_cifg(op):
+        "Must not use CIFG"
+        cifg = None not in op.inputs[2:5] + op.inputs[6:9]
+        cifg = cifg and op.inputs[1] is None
+        cifg = cifg and op.inputs[5] is None
+        return not cifg, "Op uses CIFG"
+
+    @staticmethod
+    def constraint_lstm_no_peep_hole(op):
+        "Must not use Peephole"
+        valid = all([tens is None for tens in op.inputs[9:12]])
+        return valid, "Op uses peephole"
+
+    @staticmethod
+    def constraint_lstm_no_projection(op):
+        "Must not use Projection"
+        valid = all([tens is None for tens in op.inputs[16:18]])
+        return valid, "Op uses projection"
+
+    @staticmethod
+    def constraint_lstm_no_normalisation(op):
+        "Must not use Normalisation"
+        valid = all([tens is None for tens in op.inputs[20:24]])
+        return valid, "Op uses normalisation"
+
+    @staticmethod
+    def constraint_lstm_weights(op):
+        "All input and recurrent weights must be available"
+        valid = None not in op.inputs[1:9]
+        return valid, "Op has missing weights"
```

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tflite_writer.py` & `ethos-u-vela-3.8.0/ethosu/vela/tflite_writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from .tflite import OperatorCode
 from .tflite import QuantizationParameters
 from .tflite import SubGraph
 from .tflite import Tensor
 from .tflite_mapping import builtin_operator_inv_map
 from .tflite_mapping import BuiltinOperator
 from .tflite_mapping import datatype_inv_map
+from .tflite_mapping import optype_to_builtintype
 
 # the python flatbuffer interface is missing a method to add in file identifier. patching it in here:
 
 tflite_version = 3
 tflite_file_identifier = "TFL" + str(tflite_version)
 
 
@@ -70,52 +71,49 @@
         return v
     except TypeError:
         return [v]
 
 
 class TFLiteSerialiser:
 
-    BUF_IDX_SCRATCH = 0  # Always assign scratch to buffer 0
-    BUF_IDX_SCRATCH_FAST = 1  # Always assign scratch_fast to buffer 1
-    BUF_IDX_START = 2  # Unique buffer id for every tensor in all subgraphs
+    # The 0th buffer is always by default an empty buffer that can be used by tensors
+    # without any constant data
+    BUF_IDX_ZERO = 0
+    BUF_IDX_START = 1
 
     def __init__(self, nng):
         self.builder = flatbuffers.Builder(0)
         self.nng = nng
 
         self.buf_idx = TFLiteSerialiser.BUF_IDX_START
         self.buffers_to_write = []  # have an empty array there
         self.tensor_map_all = []  # Keep track of all subgraphs
         self.tensor_map_sg = []  # Keep track of one subgraph
 
         self.ops_to_ignore = (Op.Const, Op.Placeholder, Op.SubgraphInput)
 
-        self.tensors_to_reshape = {}
-
         self.subgraphs_to_write = [sg for sg in self.nng.subgraphs if sg.placement == PassPlacement.Cpu]
 
         all_ops = []
         for sg in self.subgraphs_to_write:
             for ps in sg.passes:
                 for op in ps.ops:
                     if op.type not in self.ops_to_ignore:
                         # swap from nng input indexing to TensorFlow Lite input indexing
                         self.align_nng_inputs_to_tflite(op)
                         all_ops.append(op)
-                    if op.type.is_conv2d_op() or op.type.is_depthwise_conv2d_op():
-                        # If values are None op has non-constant weights
-                        if op.inputs[1].values is not None:
-                            self.tensors_to_reshape[op.inputs[1]] = (3, 0, 1, 2)
-                    if op.type == Op.FullyConnected:
-                        # If values are None op has non-constant weights
-                        if op.inputs[1].values is not None:
-                            self.tensors_to_reshape[op.inputs[1]] = (1, 0)
+                    if op.type.is_conv2d_op() or op.type.is_depthwise_conv2d_op() or op.type == Op.FullyConnected:
+                        # Op is run on CPU, make sure original tensor are written back
+                        # instead of the cloned/reshaped (see tflite_reader)
+                        for idx, inp in enumerate(op.inputs):
+                            if inp is not None and inp.src_tensor is not None:
+                                op.inputs[idx] = inp.src_tensor
 
-        # list of tuple(Op, string); the custom code is only used for 3rd party custom operators
-        self.operator_codes = sorted(set((op.type, op.attrs.get("custom_code", "")) for op in all_ops))
+        # list of tuple(Op, string, op.version); the custom code is only used for 3rd party custom operators
+        self.operator_codes = sorted(set((op.type, op.attrs.get("custom_code", ""), op.version) for op in all_ops))
         self.operator_code_map = {}
 
     def align_nng_inputs_to_tflite(self, op):
         from_indices = op.type.info.indices
         _, _, to_indices = builtin_operator_inv_map[op.type]
         op.inputs = align_inputs_indices(from_indices, to_indices, op.inputs)
 
@@ -160,30 +158,29 @@
         else:
             scratch_tensor_mem_area = None  # all tensors are initialised to MemArea.Unknown
 
         buffer_map = {}
 
         for tens in tensors:
             # Set buffer ids depending on allocation
-            if tens.is_allocated_in_tensor_arena(scratch_tensor_mem_area):
-                buffer_map[tens] = TFLiteSerialiser.BUF_IDX_SCRATCH
-            elif tens.mem_type == MemType.Scratch_fast:
-                # For Scratch_fast when not co-allocated with scratch in the TensorArena:
-                buffer_map[tens] = TFLiteSerialiser.BUF_IDX_SCRATCH_FAST
+            if tens.is_allocated_in_tensor_arena(scratch_tensor_mem_area) or tens.mem_type == MemType.Scratch_fast:
+                # Tensor allocated in the scratch areas, does not have any constant data and can
+                # therefore all point to the empty buffer (zero)
+                buffer_map[tens] = TFLiteSerialiser.BUF_IDX_ZERO
             else:
                 buffer_map[tens] = self.buf_idx
                 self.buf_idx += 1
 
         # Initialize/extend buffers_to_write to a length equal to number of buffers so
         # they can be appended at the correct index during tensor serialization
         self.buffers_to_write += [None] * (self.buf_idx)
 
         return buffer_map
 
-    def serialise_operator_code(self, idx, op_type, custom_code):
+    def serialise_operator_code(self, idx, op_type, custom_code, version):
         builder = self.builder
         custom_code_offset = None
         if op_type == Op.Custom:
             tf_code, opt_serializer, _ = builtin_operator_inv_map[op_type]
             custom_code_offset = builder.CreateString(custom_code)
         else:
             assert (
@@ -206,14 +203,15 @@
             self.operator_code_map[op_type][custom_code] = (idx, tf_code, opt_serializer)
         else:
             self.operator_code_map[op_type] = (idx, tf_code, opt_serializer)
 
         OperatorCode.OperatorCodeStart(builder)
         OperatorCode.OperatorCodeAddDeprecatedBuiltinCode(builder, tf_code if tf_code < 127 else 127)
         OperatorCode.OperatorCodeAddBuiltinCode(builder, tf_code)
+        OperatorCode.OperatorCodeAddVersion(builder, version)
         if custom_code_offset is not None:
             OperatorCode.OperatorCodeAddCustomCode(builder, custom_code_offset)
 
         return OperatorCode.OperatorCodeEnd(builder)
 
     def serialise_quantization_parameters(self, quant):
         builder = self.builder
@@ -254,24 +252,18 @@
             # shapes have changed size, therefore assume that the latest (modified) shape is correct
             tens_shape = tens.shape
         else:
             # shapes have not changed size, therefore the original shape is valid
             tens_shape = tens.original_shape
         values = tens.values
 
-        if values is None:
-            values = np.empty(shape=(0), dtype=np.uint8)
-
-        if tens in self.tensors_to_reshape:
-            reorder = self.tensors_to_reshape[tens]
-            tens_shape = [tens_shape[idx] for idx in reorder]
-            values = values.transpose(reorder)
-
         buf_id = self.buffer_map[tens]
-        self.buffers_to_write[buf_id] = values.flatten().view(np.uint8)
+        # Sanity check that if buffer 0 is used there must not be any data
+        assert not (buf_id == TFLiteSerialiser.BUF_IDX_ZERO and values is not None)
+        self.buffers_to_write[buf_id] = None if values is None else values.flatten().view(np.uint8)
 
         shape = self.write_int_vector(tens_shape)
 
         name = builder.CreateString(tens.name)
         quant = self.serialise_quantization_parameters(tens.quantization)
 
         Tensor.TensorStart(builder)
@@ -306,33 +298,46 @@
         else:
             op_idx, tflop, opt_serializer = self.operator_code_map[op.type]
 
         builtin_opt_offset = None
         custom_opt_offset = None
         if opt_serializer is not None:
             attrs = dict(op.attrs)
-            if "strides" in attrs:
-                attrs["stride_h"] = attrs["strides"][1]
-                attrs["stride_w"] = attrs["strides"][2]
-            if "ksize" in attrs:
-                attrs["filter_height"] = attrs["ksize"][1]
-                attrs["filter_width"] = attrs["ksize"][2]
-            if "dilation" in attrs:
-                attrs["dilation_h_factor"] = attrs["dilation"][1]
-                attrs["dilation_w_factor"] = attrs["dilation"][2]
-            if "channel_multiplier" in attrs:
-                attrs["depth_multiplier"] = attrs["channel_multiplier"]
+            if op.run_on_npu:
+                if "strides" in attrs:
+                    attrs["stride_h"] = attrs["strides"][1]
+                    attrs["stride_w"] = attrs["strides"][2]
+                if "ksize" in attrs:
+                    attrs["filter_height"] = attrs["ksize"][1]
+                    attrs["filter_width"] = attrs["ksize"][2]
+                if "dilation" in attrs:
+                    attrs["dilation_h_factor"] = attrs["dilation"][1]
+                    attrs["dilation_w_factor"] = attrs["dilation"][2]
+                if "channel_multiplier" in attrs:
+                    attrs["depth_multiplier"] = attrs["channel_multiplier"]
+                attrs["fused_activation_function"] = op.activation.op_type if op.activation is not None else None
+
+            # Serialize VarHandleOptions (only op that have attributes with type String)
             if "container" in attrs:
                 attrs["container"] = builder.CreateString(attrs["container"])
             if "shared_name" in attrs:
                 attrs["shared_name"] = builder.CreateString(attrs["shared_name"])
-            attrs["fused_activation_function"] = op.activation.op_type if op.activation is not None else None
 
             builtin_opt_offset, custom_opt_offset = opt_serializer.serialize(builder, attrs)
 
+            # report any missing attributes that could not be written during serialize().
+            # operators that have been created internally (i.e. not created as part of reading an input network) may not
+            # have the write error attribute
+            attribute_write_error = attrs.get("attribute_write_error", [])
+            if len(attribute_write_error) != 0:
+                print(
+                    f"Warning: Could not write the following attributes to {optype_to_builtintype(op.type)}"
+                    f" '{op.name}' {opt_serializer.name} field: {', '.join(attribute_write_error)}"
+                )
+
         mutating_variable_inputs_offset = self.write_byte_vector([])
         Operator.OperatorStart(builder)
         Operator.OperatorAddOpcodeIndex(builder, op_idx)
         Operator.OperatorAddInputs(builder, inputs_offset)
         Operator.OperatorAddOutputs(builder, outputs_offset)
         Operator.OperatorAddIntermediates(builder, intermediates_offset)
 
@@ -449,15 +454,18 @@
         Metadata.MetadataAddBuffer(builder, metadata[1])
 
         return Metadata.MetadataEnd(builder)
 
     def serialise_model(self):
         builder = self.builder
         operator_code_offset = self.write_offset_vector(
-            [self.serialise_operator_code(idx, optype, code) for idx, (optype, code) in enumerate(self.operator_codes)]
+            [
+                self.serialise_operator_code(idx, optype, code, version)
+                for idx, (optype, code, version) in enumerate(self.operator_codes)
+            ]
         )
 
         description = builder.CreateString("Vela Optimised")
 
         subgraph_offset = self.write_offset_vector(
             [self.serialise_subgraph(sg, builder.CreateString(sg.name)) for sg in self.subgraphs_to_write]
         )
```

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tosa/ArithmeticRightShiftAttribute.py` & `ethos-u-vela-3.8.0/ethosu/vela/tosa/ArithmeticRightShiftAttribute.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tosa/AxisAttribute.py` & `ethos-u-vela-3.8.0/ethosu/vela/tosa/AxisAttribute.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tosa/ClampAttribute.py` & `ethos-u-vela-3.8.0/ethosu/vela/tosa/ClampAttribute.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tosa/CondIfAttribute.py` & `ethos-u-vela-3.8.0/ethosu/vela/tosa/CondIfAttribute.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tosa/ConvAttribute.py` & `ethos-u-vela-3.8.0/ethosu/vela/tosa/ConvAttribute.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tosa/ConvQuantInfo.py` & `ethos-u-vela-3.8.0/ethosu/vela/tosa/ConvQuantInfo.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tosa/MatMulQuantInfo.py` & `ethos-u-vela-3.8.0/ethosu/vela/tosa/MatMulQuantInfo.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tosa/MulAttribute.py` & `ethos-u-vela-3.8.0/ethosu/vela/tosa/MulAttribute.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tosa/Op.py` & `ethos-u-vela-3.8.0/ethosu/vela/tosa/Op.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tosa/PadQuantInfo.py` & `ethos-u-vela-3.8.0/ethosu/vela/tosa/PadQuantInfo.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tosa/PoolAttribute.py` & `ethos-u-vela-3.8.0/ethosu/vela/tosa/PoolAttribute.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tosa/ReluNAttribute.py` & `ethos-u-vela-3.8.0/ethosu/vela/tosa/ReluNAttribute.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tosa/RescaleAttribute.py` & `ethos-u-vela-3.8.0/ethosu/vela/tosa/RescaleAttribute.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tosa/ReshapeAttribute.py` & `ethos-u-vela-3.8.0/ethosu/vela/tosa/ReshapeAttribute.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tosa/ResizeAttribute.py` & `ethos-u-vela-3.8.0/ethosu/vela/tosa/ResizeAttribute.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tosa/SliceAttribute.py` & `ethos-u-vela-3.8.0/ethosu/vela/tosa/SliceAttribute.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tosa/TileAttribute.py` & `ethos-u-vela-3.8.0/ethosu/vela/tosa/TileAttribute.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tosa/TosaBasicBlock.py` & `ethos-u-vela-3.8.0/ethosu/vela/tosa/TosaBasicBlock.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tosa/TosaGraph.py` & `ethos-u-vela-3.8.0/ethosu/vela/tosa/TosaGraph.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tosa/TosaOperator.py` & `ethos-u-vela-3.8.0/ethosu/vela/tosa/TosaOperator.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tosa/TosaTensor.py` & `ethos-u-vela-3.8.0/ethosu/vela/tosa/TosaTensor.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tosa/TransposeConvAttribute.py` & `ethos-u-vela-3.8.0/ethosu/vela/tosa/TransposeConvAttribute.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tosa/UnaryQuantInfo.py` & `ethos-u-vela-3.8.0/ethosu/vela/tosa/UnaryQuantInfo.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tosa/Version.py` & `ethos-u-vela-3.8.0/ethosu/vela/tosa/Version.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tosa/WhileLoopAttribute.py` & `ethos-u-vela-3.8.0/ethosu/vela/tosa/WhileLoopAttribute.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tosa_graph_optimiser.py` & `ethos-u-vela-3.8.0/ethosu/vela/tosa_graph_optimiser.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,27 +15,27 @@
 # limitations under the License.
 #
 # Description:
 # Early optimisation of the TOSA based network graph, using the rewrite_graph module to do the traversal of the graph.
 import numpy as np
 
 from . import rewrite_graph
-from .api import NpuRoundingMode
 from .data_type import DataType
 from .debug_database import DebugDatabase
 from .graph_optimiser_util import bypass_memory_only_ops
 from .graph_optimiser_util import calc_explicit_padding
 from .graph_optimiser_util import convert_depthwise_to_conv
-from .graph_optimiser_util import convert_to_lut
 from .graph_optimiser_util import move_splitsliceread_to_consumer
 from .graph_optimiser_util import needed_total_padding
 from .graph_optimiser_util import set_ifm_ofm_op_shapes
 from .graph_optimiser_util import set_tensor_equivalence
+from .lut import convert_to_lut
 from .operation import ExplicitScaling
 from .operation import Op
+from .operation import RoundingMode
 from .operation_util import create_add_nop
 from .operation_util import create_avgpool_nop
 from .operation_util import create_pad_nop
 from .shape4d import Shape4D
 from .tensor import create_const_tensor
 from .tensor import create_equivalence_id
 from .tensor import shape_num_elements
@@ -111,15 +111,15 @@
 
         kernel_wh = op.kernel.elements_wh()
         k = 32 - count_leading_zeros(kernel_wh - 1)
         numerator = np.int64(((1 << 30) + 1) << k)
         multiplier.append(numerator // kernel_wh)
         shift.append(30 + k)
 
-        op.rounding_mode = NpuRoundingMode.NATURAL
+        op.rounding_mode = RoundingMode.HalfUp
         op.explicit_scaling = ExplicitScaling(False, shift, multiplier)
     return op
 
 
 def remove_const_transpose(op, arch, nng):
     if op.type == Op.Transpose:
         removed = False
@@ -395,17 +395,17 @@
             assert m >= 0
             assert 2 <= s <= 62
             # TODO these are the HW limitations
             assert 0 <= s < (1 << 6)
         explicit_scaling = ExplicitScaling(per_channel, shift, multiplier)
 
         if double_round and scale32:
-            rounding_mode = NpuRoundingMode.TFL
+            rounding_mode = RoundingMode.TFLite
         else:
-            rounding_mode = NpuRoundingMode.NATURAL
+            rounding_mode = RoundingMode.HalfUp
 
         if prev_op.type.is_depthwise_conv2d_op() or prev_op.type.is_conv2d_op() or prev_op.type == Op.FullyConnected:
             assert len(multiplier) == len(shift) == len(prev_op.bias.values)
 
             if ifm.dtype == DataType.int32 and per_channel:
                 prev_op.explicit_scaling = explicit_scaling
                 prev_op.rounding_mode = rounding_mode
```

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tosa_mapping.py` & `ethos-u-vela-3.8.0/ethosu/vela/tosa_mapping.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tosa_model_semantic.py` & `ethos-u-vela-3.8.0/ethosu/vela/tosa_model_semantic.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tosa_reader.py` & `ethos-u-vela-3.8.0/ethosu/vela/tosa_reader.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/tosa_supported_operators.py` & `ethos-u-vela-3.8.0/ethosu/vela/tosa_supported_operators.py`

 * *Files identical despite different names*

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/vela.py` & `ethos-u-vela-3.8.0/ethosu/vela/vela.py`

 * *Files 3% similar despite different names*

```diff
@@ -171,26 +171,51 @@
         print(f"      Total Size = {sg_size} KiB")
         print(f"      SRAM Memory Used = {sg.memory_used.get(MemArea.Sram, 0) / 1024.0} KiB")
         max_sg_size = max(sg_size, max_sg_size)
 
     print(f"   Maximum NNG Subgraph Size = {max_sg_size} KiB")
 
 
+def generate_license():
+    lines = [
+        "<!--",
+        "SPDX-FileCopyrightText: Copyright 2020-2023 Arm Limited and/or its affiliates <open-source-office@arm.com>",
+        "",
+        "SPDX-License-Identifier: Apache-2.0",
+        "",
+        "Licensed under the Apache License, Version 2.0 (the License); you may",
+        "not use this file except in compliance with the License.",
+        "You may obtain a copy of the License at",
+        "",
+        "www.apache.org/licenses/LICENSE-2.0",
+        "",
+        "Unless required by applicable law or agreed to in writing, software",
+        "distributed under the License is distributed on an AS IS BASIS, WITHOUT",
+        "WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.",
+        "See the License for the specific language governing permissions and",
+        "limitations under the License.",
+        "-->",
+        "",
+    ]
+    return lines
+
+
 def generate_supported_ops():
     # Exclude network type from generation by adding value to exclude list.
     # To easily exclude NetworkType from generated documentation.
     exclude_generation_network_type_value = [NetworkType.TOSA.value]
 
     def _exclude_list_names(constraint, exclude_list):
         constraints_excluded_names = [
             optype_to_builtintype(op) for op, exclude_constraint in exclude_list if constraint in exclude_constraint
         ]
         return f" - [{', '.join(sorted(constraints_excluded_names))}]" if constraints_excluded_names else ""
 
-    lines = [
+    lines = generate_license()
+    lines += [
         "# Supported Ops",
         "",
         "This file was automatically generated by Vela using the `--supported-ops-report` parameter.  ",
         f"Vela version: `{__version__}`",
         "",
         "This file complies with",
         "[**Gitiles Markdown syntax**](https://github.com/google/gitiles/blob/master/Documentation/markdown.md)",
@@ -368,14 +393,15 @@
         )
         parser.add_argument(
             "--verbose-register-command-stream", action="store_true", help="Verbose register command stream"
         )
         parser.add_argument("--verbose-operators", action="store_true", help="Verbose operator list")
         parser.add_argument("--verbose-weights", action="store_true", help="Verbose weights information")
         parser.add_argument("--verbose-performance", action="store_true", help="Verbose performance information")
+        parser.add_argument("--verbose-progress", action="store_true", help="Verbose progress information")
         parser.add_argument(
             "--show-cpu-operations", action="store_true", help="Show the operations that fall back to the CPU"
         )
         parser.add_argument("--timing", action="store_true", help="Time the compiler doing operations")
         parser.add_argument(
             "--force-symmetric-int-weights",
             action="store_true",
@@ -551,27 +577,29 @@
             verbose_tensor_format=args.verbose_tensor_format,
             verbose_allocation=args.verbose_allocation,
             verbose_high_level_command_stream=args.verbose_high_level_command_stream,
             verbose_register_command_stream=args.verbose_register_command_stream,
             verbose_operators=args.verbose_operators,
             verbose_weights=args.verbose_weights,
             verbose_performance=args.verbose_performance,
+            verbose_progress=args.verbose_progress,
             show_cpu_operations=args.show_cpu_operations,
             tensor_allocator=args.tensor_allocator,
             timing=args.timing,
             force_symmetric_int_weights=args.force_symmetric_int_weights,
             output_dir=args.output_dir,
             cpu_tensor_alignment=args.cpu_tensor_alignment,
             hillclimb_max_iterations=args.hillclimb_max_iterations,
         )
 
         scheduler_options = scheduler.SchedulerOptions(
             optimization_strategy=args.optimise,
             sram_target=arch.arena_cache_size,
             verbose_schedule=args.verbose_schedule,
+            verbose_progress=args.verbose_progress,
         )
 
         model_reader_options = model_reader.ModelReaderOptions()
 
         nng = process(
             args.network, args.enable_debug_db, arch, model_reader_options, compiler_options, scheduler_options
         )
```

### Comparing `ethos-u-vela-3.7.0/ethosu/vela/weight_compressor.py` & `ethos-u-vela-3.8.0/ethosu/vela/weight_compressor.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,16 +28,18 @@
 from .architecture_features import Accelerator
 from .architecture_features import ArchitectureFeatures
 from .data_type import DataType
 from .errors import UnsupportedFeatureError
 from .numeric_util import round_up
 from .operation import NpuBlockType
 from .operation import Op
+from .operation import RoundingMode
 from .scaling import quantise_scale
 from .scaling import reduced_quantise_scale
+from .tensor import QuantizationParameters
 from .tensor import Tensor
 from .tensor import TensorFormat
 from .tensor import TensorPurpose
 
 # Handle any errors thrown by NumPy while importing mlw_codec module
 try:
     from ethosu import mlw_codec
@@ -231,102 +233,101 @@
 
 def core_deinterleave(hwio, core, ncores):
     # Put weights back into OHWI
     ohwi = np.transpose(hwio, (3, 0, 1, 2))
     return ohwi[core : ohwi.shape[0] : ncores]
 
 
-def _prepare_scale_and_bias(arch, tens, rescale_for_faf, explicit_scaling):
+def _get_input_quantization(op):
+    quant = op.get_input_quantization()
+    if not quant:
+        quant = QuantizationParameters(scale_f32=1.0, zero_point=0)
+    return quant
+
+
+def _get_output_quantization(op):
+    quant = op.get_output_quantization()
+    if not quant:
+        quant = QuantizationParameters(scale_f32=1.0, zero_point=0)
+    return quant
+
+
+def _prepare_scale_and_bias(arch, tens, explicit_scaling):
     assert tens.purpose in [TensorPurpose.FeatureMap, TensorPurpose.FSBias]
     assert tens.format == TensorFormat.NHWC
     # the connected operator should expect a bias input unless it is a FullyConnected
     assert tens.consumer_list[0].type.needs_bias()
     # the input bias tensor is the same as that connected to the operator
     bias_tens = tens.consumer_list[0].bias
     assert tens is bias_tens
 
     # the operator should only have a single output
     assert len(tens.consumer_list[0].outputs) == 1
     biases = tens.values
 
     first_consumer_op = tens.consumer_list[0]
     ifm_dtype = first_consumer_op.inputs[0].dtype
-    ifm_scale = first_consumer_op.get_input_quantization().scale_f32
-    ofm_scale = first_consumer_op.get_output_quantization().scale_f32
+    ifm_scale = _get_input_quantization(first_consumer_op).scale_f32
+    ofm_scale = _get_output_quantization(first_consumer_op).scale_f32
     weight_scales = first_consumer_op.inputs[1].quantization.scale_f32
 
     # biases can have multiple consumers for rnn cells. if so, then check that they are all the same
     for op in tens.consumer_list[1:]:
-        assert ifm_scale == op.get_input_quantization().scale_f32
-        assert ofm_scale == op.get_output_quantization().scale_f32
+        assert ifm_scale == _get_input_quantization(op).scale_f32
+        assert ofm_scale == _get_output_quantization(op).scale_f32
         assert weight_scales == op.inputs[1].quantization.scale_f32
 
     if not hasattr(weight_scales, "__iter__"):
         # If weight_scales is not already an iterable make it into a list
         weight_scales = [weight_scales]
 
     # Convert scales to np.double (from np.float32) to conform to TensorFlow Lite which
     # uses double during scaling calculations
-    # TensorFlow Lite casts the scales slightly differently for uint8 and int8
-    if not rescale_for_faf:
-        if ifm_dtype == DataType.uint8:
-            # for some cases of the Mean operator, the scale must be calculated differently to match reference
-            if first_consumer_op.low_precision_scaling:
-                scales = [
-                    np.double(np.single(ifm_scale) / (np.single(weight_scale) * np.single(ofm_scale)))
-                    for weight_scale in weight_scales
-                ]
-            else:
-                scales = [np.double(ifm_scale * weight_scale) / np.double(ofm_scale) for weight_scale in weight_scales]
-        elif ifm_dtype == DataType.int8 or ifm_dtype == DataType.int16:
-            scales = [
-                (np.double(ifm_scale) * np.double(weight_scale)) / np.double(ofm_scale)
-                for weight_scale in weight_scales
-            ]
-        else:
-            raise UnsupportedFeatureError(f"Compression of {ifm_dtype} is not implemented; Tensor: '{tens.name}'")
+    # TensorFlow Lite casts the scales slightly differently for uint8 and int8 as well as
+    # for FullyConnected operators
+    if ifm_dtype == DataType.uint8 or first_consumer_op.original_type == Op.FullyConnected:
+        scales = [np.double(ifm_scale * weight_scale) / np.double(ofm_scale) for weight_scale in weight_scales]
+    elif ifm_dtype == DataType.int8 or ifm_dtype == DataType.int16:
+        scales = [
+            (np.double(ifm_scale) * np.double(weight_scale)) / np.double(ofm_scale) for weight_scale in weight_scales
+        ]
     else:
-        if ifm_dtype == DataType.uint8:
-            scales = [np.double(ifm_scale * weight_scale * 0x3000) for weight_scale in weight_scales]
-        elif ifm_dtype == DataType.int8 or ifm_dtype == DataType.int16:
-            scales = [(np.double(ifm_scale * 0x3000) * np.double(weight_scale)) for weight_scale in weight_scales]
-        else:
-            raise UnsupportedFeatureError(f"Compression of {ifm_dtype} is not implemented; Tensor: '{tens.name}'")
+        raise UnsupportedFeatureError(f"Compression of {ifm_dtype} is not implemented; Tensor: '{tens.name}'")
 
     if explicit_scaling:
         assert len(explicit_scaling.shift) == len(explicit_scaling.multiplier)
         quantised_scales = [(int(m), int(s)) for s, m in zip(explicit_scaling.shift, explicit_scaling.multiplier)]
     else:
         # quantise all of the weight scales into (scale_factor, shift)
         if ifm_dtype == DataType.int16 and bias_tens.dtype == DataType.int64:
             # Reference uses reduced scaling for int16 with int64 bias
             quantised_scales = [reduced_quantise_scale(scale) for scale in scales]
         else:
             quantised_scales = [quantise_scale(scale) for scale in scales]
 
-    # Check the output quantisation to see if the scale value needs increasing to the next one
-    if first_consumer_op.get_output_quantization().next_after:
+    # Rounding away from zero requires the "next after" floating point value to be set on the output quantisation
+    if first_consumer_op.rounding_mode == RoundingMode.AwayZero:
         for i, quant_scale in enumerate(quantised_scales):
             q_scale, q_shift = quant_scale
             quantised_scales[i] = (q_scale + 1, q_shift)
 
     # If only 1 quantised scale is used, repeat that value for the length of the biases
     if len(quantised_scales) == 1:
         quantised_scales = [quantised_scales[0]] * len(biases)
 
     return quantised_scales, biases
 
 
 def encode_weight_and_scale_tensor(
-    arch, op, weight_tens, scale_tens, kernel, block_config, depth_offsets, rescale_for_faf=False
+    arch, op, weight_tens, scale_tens, kernel, block_config, depth_offsets
 ) -> Tuple[Optional[NpuWeightTensor], Optional[NpuWeightTensor]]:
     npu_block_type = op.type.npu_block_type
 
-    ifm_scale = scale_tens and scale_tens.consumer_list[0].get_input_quantization().scale_f32
-    ofm_scale = scale_tens and scale_tens.consumer_list[0].get_output_quantization().scale_f32
+    ifm_scale = scale_tens and _get_input_quantization(scale_tens.consumer_list[0]).scale_f32
+    ofm_scale = scale_tens and _get_output_quantization(scale_tens.consumer_list[0]).scale_f32
 
     wcc = create_weight_compression_config(
         weight_tens, npu_block_type, block_config.ofm_block.depth, hash(str(depth_offsets)), kernel.dilation
     )
 
     scc = ScaleCompressionConfig(scale_tens and scale_tens.value_id, ifm_scale, ofm_scale)
 
@@ -394,15 +395,15 @@
 
     encoded_stream = bytearray()
     double_buffer_sizes = [0, 0]
     is_depthwise = npu_block_type == NpuBlockType.ConvolutionDepthWise
 
     # Bias & scale
     if do_scales:
-        quantised_scales, biases = _prepare_scale_and_bias(arch, scale_tens, rescale_for_faf, op.explicit_scaling)
+        quantised_scales, biases = _prepare_scale_and_bias(arch, scale_tens, op.explicit_scaling)
         scale_tens.element_size_bytes = 10
 
     # Slice the weight stream up depth-ways into bricks and compress
     full_ofm_depth = weight_tens.values.shape[-1]
     ofm_block_depth = block_config.ofm_block.depth
 
     weight_range_index = 0
```

### Comparing `ethos-u-vela-3.7.0/pyproject.toml` & `ethos-u-vela-3.8.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -24,33 +24,42 @@
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: POSIX :: Linux",
     "Operating System :: Microsoft :: Windows :: Windows 10",
     "Programming Language :: C",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.9",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Software Development :: Compilers",
 ]
 keywords = ["ethos-u", "vela compiler", "tflite", "npu"]
 dependencies = [
     "flatbuffers==2.0.7",
     "numpy<=1.21.3; python_version<='3.7'",
     "numpy; python_version>'3.7'",
-    "lxml>=4.5.1"
+    "lxml>=4.5.2"
 ]
 dynamic = ["readme", "version"]
 
+[project.optional-dependencies]
+dev = [
+    "pytest",
+    "pytest-cov",
+    "pre-commit",
+    "build",
+    "setuptools_scm[toml]~=7.1.0"
+]
+
 [project.urls]
 Homepage = "https://git.mlplatform.org/ml/ethos-u/ethos-u-vela.git/"
 
 [project.scripts]
 vela = "ethosu.vela.vela:main"
 
 [build-system]
 requires = [
     "numpy<=1.21.3; python_version<='3.7'",
     "numpy; python_version>'3.7'",
-    "setuptools_scm[toml]<6"
+    "setuptools_scm[toml]~=7.1.0"
 ]
 build-backend = "setuptools.build_meta"
```

### Comparing `ethos-u-vela-3.7.0/setup.py` & `ethos-u-vela-3.8.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 # Packaging for the Vela compiler
 import os
 import re
 
 from setuptools import Extension
 from setuptools import setup
 from setuptools.command.build_ext import build_ext
+from setuptools_scm import get_version
 
 
 class BuildExtension(build_ext):
     def finalize_options(self):
         build_ext.finalize_options(self)
         import builtins
 
@@ -37,15 +38,15 @@
         self.include_dirs.append(np.get_include())
 
 
 # Read the contents of README.md file
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
-    tag = "3.7.0"
+    tag = get_version()
     url = f"https://review.mlplatform.org/plugins/gitiles/ml/ethos-u/ethos-u-vela/+/refs/tags/{tag}/"
     # Find all markdown links that match the format:  [text](link)
     for match, link in re.findall(r"(\[.+?\]\((.+?)\))", long_description):
         # If the link is a file that exists, replace it with the web link to the file instead
         if os.path.exists(os.path.join(this_directory, link)):
             url_link = match.replace(link, url + link)
             long_description = long_description.replace(match, url_link)
```

