# Comparing `tmp/dagster-1.3.5.tar.gz` & `tmp/dagster-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-1.3.5.tar", last modified: Thu May 18 20:38:25 2023, max compression
+gzip compressed data, was "dagster-1.3.6.tar", last modified: Thu May 25 17:17:08 2023, max compression
```

## Comparing `dagster-1.3.5.tar` & `dagster-1.3.6.tar`

### file list

```diff
@@ -1,626 +1,628 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.105472 dagster-1.3.5/
--rw-r--r--   0 root         (0) root         (0)      549 2023-05-18 20:38:07.000000 dagster-1.3.5/COPYING
--rw-r--r--   0 root         (0) root         (0)    11344 2023-05-18 20:38:07.000000 dagster-1.3.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      485 2023-05-18 20:38:07.000000 dagster-1.3.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8790 2023-05-18 20:38:25.105472 dagster-1.3.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7167 2023-05-18 20:38:07.000000 dagster-1.3.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.029472 dagster-1.3.5/dagster/
--rw-r--r--   0 root         (0) root         (0)    26157 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/__init__.py
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/__main__.py
--rw-r--r--   0 root         (0) root         (0)     5456 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_annotations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.033472 dagster-1.3.5/dagster/_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      731 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_api/get_server_id.py
--rw-r--r--   0 root         (0) root         (0)     2147 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_api/list_repositories.py
--rw-r--r--   0 root         (0) root         (0)      531 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_api/notebook_data.py
--rw-r--r--   0 root         (0) root         (0)     2882 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_api/snapshot_execution_plan.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_api/snapshot_job.py
--rw-r--r--   0 root         (0) root         (0)     5479 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_api/snapshot_partition.py
--rw-r--r--   0 root         (0) root         (0)     1668 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_api/snapshot_repository.py
--rw-r--r--   0 root         (0) root         (0)     2727 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_api/snapshot_schedule.py
--rw-r--r--   0 root         (0) root         (0)     2901 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_api/snapshot_sensor.py
--rw-r--r--   0 root         (0) root         (0)      478 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_builtins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.033472 dagster-1.3.5/dagster/_check/
--rw-r--r--   0 root         (0) root         (0)     1352 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_check/README.md
--rw-r--r--   0 root         (0) root         (0)    51637 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_check/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.033472 dagster-1.3.5/dagster/_cli/
--rw-r--r--   0 root         (0) root         (0)     1101 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27119 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_cli/api.py
--rw-r--r--   0 root         (0) root         (0)     8186 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_cli/asset.py
--rw-r--r--   0 root         (0) root         (0)     2300 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_cli/config_scaffolder.py
--rw-r--r--   0 root         (0) root         (0)     3533 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_cli/debug.py
--rw-r--r--   0 root         (0) root         (0)     5695 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_cli/dev.py
--rw-r--r--   0 root         (0) root         (0)     2252 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_cli/instance.py
--rw-r--r--   0 root         (0) root         (0)    29822 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_cli/job.py
--rw-r--r--   0 root         (0) root         (0)     1695 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_cli/load_handle.py
--rw-r--r--   0 root         (0) root         (0)     5852 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_cli/project.py
--rw-r--r--   0 root         (0) root         (0)     5135 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_cli/run.py
--rw-r--r--   0 root         (0) root         (0)    19909 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_cli/schedule.py
--rw-r--r--   0 root         (0) root         (0)    15661 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_cli/sensor.py
--rw-r--r--   0 root         (0) root         (0)     1409 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_cli/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.033472 dagster-1.3.5/dagster/_cli/workspace/
--rw-r--r--   0 root         (0) root         (0)      180 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_cli/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28391 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_cli/workspace/cli_target.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.037473 dagster-1.3.5/dagster/_config/
--rw-r--r--   0 root         (0) root         (0)     3186 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3403 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    15864 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/config_type.py
--rw-r--r--   0 root         (0) root         (0)    19601 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/errors.py
--rw-r--r--   0 root         (0) root         (0)     1783 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/evaluate_value_result.py
--rw-r--r--   0 root         (0) root         (0)    15269 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/field.py
--rw-r--r--   0 root         (0) root         (0)    16880 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/field_utils.py
--rw-r--r--   0 root         (0) root         (0)     9466 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/post_process.py
--rw-r--r--   0 root         (0) root         (0)      855 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/primitive_mapping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.037473 dagster-1.3.5/dagster/_config/pythonic_config/
--rw-r--r--   0 root         (0) root         (0)    71109 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/pythonic_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/pythonic_config/attach_other_object_to_context.py
--rw-r--r--   0 root         (0) root         (0)     6217 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/pythonic_config/typing_utils.py
--rw-r--r--   0 root         (0) root         (0)      577 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/pythonic_config/utils.py
--rw-r--r--   0 root         (0) root         (0)    12143 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/snap.py
--rw-r--r--   0 root         (0) root         (0)     3267 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/source.py
--rw-r--r--   0 root         (0) root         (0)     3528 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/stack.py
--rw-r--r--   0 root         (0) root         (0)     7772 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/traversal_context.py
--rw-r--r--   0 root         (0) root         (0)     4167 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/type_printer.py
--rw-r--r--   0 root         (0) root         (0)    17162 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_config/validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.037473 dagster-1.3.5/dagster/_core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      994 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/assets.py
--rw-r--r--   0 root         (0) root         (0)    13645 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/code_pointer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.041473 dagster-1.3.5/dagster/_core/container_context/
--rw-r--r--   0 root         (0) root         (0)      184 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/container_context/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/container_context/config.py
--rw-r--r--   0 root         (0) root         (0)     2310 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/debug.py
--rw-r--r--   0 root         (0) root         (0)     3005 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/decorator_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.053472 dagster-1.3.5/dagster/_core/definitions/
--rw-r--r--   0 root         (0) root         (0)     7626 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30229 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)    10704 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/asset_graph_subset.py
--rw-r--r--   0 root         (0) root         (0)     3816 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/asset_in.py
--rw-r--r--   0 root         (0) root         (0)    36842 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/asset_layer.py
--rw-r--r--   0 root         (0) root         (0)     5685 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/asset_out.py
--rw-r--r--   0 root         (0) root         (0)    56981 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/asset_reconciliation_sensor.py
--rw-r--r--   0 root         (0) root         (0)    18474 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/asset_selection.py
--rw-r--r--   0 root         (0) root         (0)     7164 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    64232 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/assets.py
--rw-r--r--   0 root         (0) root         (0)    24005 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/assets_job.py
--rw-r--r--   0 root         (0) root         (0)     2806 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/auto_materialize_condition.py
--rw-r--r--   0 root         (0) root         (0)     5297 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/auto_materialize_policy.py
--rw-r--r--   0 root         (0) root         (0)    16105 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/cacheable_assets.py
--rw-r--r--   0 root         (0) root         (0)    45671 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/composition.py
--rw-r--r--   0 root         (0) root         (0)     4287 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/config.py
--rw-r--r--   0 root         (0) root         (0)    10845 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/configurable.py
--rw-r--r--   0 root         (0) root         (0)    20795 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/data_time.py
--rw-r--r--   0 root         (0) root         (0)    17905 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/data_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.053472 dagster-1.3.5/dagster/_core/definitions/decorators/
--rw-r--r--   0 root         (0) root         (0)      620 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42826 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/decorators/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     4915 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/decorators/config_mapping_decorator.py
--rw-r--r--   0 root         (0) root         (0)     8250 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/decorators/graph_decorator.py
--rw-r--r--   0 root         (0) root         (0)     9444 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/decorators/hook_decorator.py
--rw-r--r--   0 root         (0) root         (0)    10676 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/decorators/job_decorator.py
--rw-r--r--   0 root         (0) root         (0)    17845 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/decorators/op_decorator.py
--rw-r--r--   0 root         (0) root         (0)    14396 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/decorators/repository_decorator.py
--rw-r--r--   0 root         (0) root         (0)     8656 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/decorators/schedule_decorator.py
--rw-r--r--   0 root         (0) root         (0)    11936 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/decorators/sensor_decorator.py
--rw-r--r--   0 root         (0) root         (0)     6695 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/decorators/source_asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     5275 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/definition_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    20546 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/definitions_class.py
--rw-r--r--   0 root         (0) root         (0)    39988 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/dependency.py
--rw-r--r--   0 root         (0) root         (0)    31576 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/events.py
--rw-r--r--   0 root         (0) root         (0)    21013 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/executor_definition.py
--rw-r--r--   0 root         (0) root         (0)    10548 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/external_asset_graph.py
--rw-r--r--   0 root         (0) root         (0)     8010 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    16195 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/freshness_policy_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    44740 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/graph_definition.py
--rw-r--r--   0 root         (0) root         (0)     6546 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/hook_definition.py
--rw-r--r--   0 root         (0) root         (0)     1515 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/hook_invocation.py
--rw-r--r--   0 root         (0) root         (0)     3205 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/inference.py
--rw-r--r--   0 root         (0) root         (0)    22898 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/input.py
--rw-r--r--   0 root         (0) root         (0)     5386 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/instigation_logger.py
--rw-r--r--   0 root         (0) root         (0)     2152 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/job_base.py
--rw-r--r--   0 root         (0) root         (0)    51147 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/job_definition.py
--rw-r--r--   0 root         (0) root         (0)    20308 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/load_assets_from_modules.py
--rw-r--r--   0 root         (0) root         (0)     6845 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/logger_definition.py
--rw-r--r--   0 root         (0) root         (0)      636 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/logger_invocation.py
--rw-r--r--   0 root         (0) root         (0)     8841 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/materialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.053472 dagster-1.3.5/dagster/_core/definitions/metadata/
--rw-r--r--   0 root         (0) root         (0)    32319 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8557 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/metadata/table.py
--rw-r--r--   0 root         (0) root         (0)    55971 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/multi_asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    20758 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/multi_dimensional_partitions.py
--rw-r--r--   0 root         (0) root         (0)       82 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/no_step_launcher.py
--rw-r--r--   0 root         (0) root         (0)    11927 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/node_container.py
--rw-r--r--   0 root         (0) root         (0)     8041 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/node_definition.py
--rw-r--r--   0 root         (0) root         (0)     2867 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/observe.py
--rw-r--r--   0 root         (0) root         (0)    22629 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/op_definition.py
--rw-r--r--   0 root         (0) root         (0)    19256 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/op_invocation.py
--rw-r--r--   0 root         (0) root         (0)     7509 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/op_selection.py
--rw-r--r--   0 root         (0) root         (0)    18908 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/output.py
--rw-r--r--   0 root         (0) root         (0)    37817 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/partition.py
--rw-r--r--   0 root         (0) root         (0)      196 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/partition_key_range.py
--rw-r--r--   0 root         (0) root         (0)    47274 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)     8811 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/partitioned_schedule.py
--rw-r--r--   0 root         (0) root         (0)     3779 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/policy.py
--rw-r--r--   0 root         (0) root         (0)    27231 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/reconstruct.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.053472 dagster-1.3.5/dagster/_core/definitions/repository_definition/
--rw-r--r--   0 root         (0) root         (0)      654 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/repository_definition/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6670 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/repository_definition/caching_index.py
--rw-r--r--   0 root         (0) root         (0)    18856 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/repository_definition/repository_data.py
--rw-r--r--   0 root         (0) root         (0)    17401 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/repository_definition/repository_data_builder.py
--rw-r--r--   0 root         (0) root         (0)    16917 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/repository_definition/repository_definition.py
--rw-r--r--   0 root         (0) root         (0)     1479 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/repository_definition/valid_definitions.py
--rw-r--r--   0 root         (0) root         (0)     5108 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/resolved_asset_deps.py
--rw-r--r--   0 root         (0) root         (0)     1336 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/resource_annotation.py
--rw-r--r--   0 root         (0) root         (0)    16162 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/resource_definition.py
--rw-r--r--   0 root         (0) root         (0)     5398 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/resource_invocation.py
--rw-r--r--   0 root         (0) root         (0)     7806 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/resource_requirement.py
--rw-r--r--   0 root         (0) root         (0)    24105 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/run_config.py
--rw-r--r--   0 root         (0) root         (0)     1445 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    15824 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/run_request.py
--rw-r--r--   0 root         (0) root         (0)    38400 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/run_status_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    36719 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/schedule_definition.py
--rw-r--r--   0 root         (0) root         (0)     5189 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/scoped_resources_builder.py
--rw-r--r--   0 root         (0) root         (0)    10837 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/selector.py
--rw-r--r--   0 root         (0) root         (0)    46037 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    14249 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/source_asset.py
--rw-r--r--   0 root         (0) root         (0)     2298 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/step_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1535 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/target.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/test_op_definition.py
--rw-r--r--   0 root         (0) root         (0)    12374 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/time_window_partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)    76525 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/time_window_partitions.py
--rw-r--r--   0 root         (0) root         (0)    15645 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/unresolved_asset_job_definition.py
--rw-r--r--   0 root         (0) root         (0)     7992 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/utils.py
--rw-r--r--   0 root         (0) root         (0)     2930 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/definitions/version_strategy.py
--rw-r--r--   0 root         (0) root         (0)    25453 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/errors.py
--rw-r--r--   0 root         (0) root         (0)     6232 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/event_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.053472 dagster-1.3.5/dagster/_core/events/
--rw-r--r--   0 root         (0) root         (0)    64981 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/events/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7783 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/events/log.py
--rw-r--r--   0 root         (0) root         (0)     1614 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/events/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.057473 dagster-1.3.5/dagster/_core/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38315 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/api.py
--rw-r--r--   0 root         (0) root         (0)    30249 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/asset_backfill.py
--rw-r--r--   0 root         (0) root         (0)    14476 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     6326 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/build_resources.py
--rw-r--r--   0 root         (0) root         (0)      224 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/bulk_actions.py
--rw-r--r--   0 root         (0) root         (0)     5587 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/compute_logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.061473 dagster-1.3.5/dagster/_core/execution/context/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/context/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21992 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/context/compute.py
--rw-r--r--   0 root         (0) root         (0)    15991 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/context/hook.py
--rw-r--r--   0 root         (0) root         (0)     9369 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/context/init.py
--rw-r--r--   0 root         (0) root         (0)    26845 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/context/input.py
--rw-r--r--   0 root         (0) root         (0)    27417 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/context/invocation.py
--rw-r--r--   0 root         (0) root         (0)     3164 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/context/logger.py
--rw-r--r--   0 root         (0) root         (0)    33974 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/context/output.py
--rw-r--r--   0 root         (0) root         (0)    44193 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/context/system.py
--rw-r--r--   0 root         (0) root         (0)    18501 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/context_creation_job.py
--rw-r--r--   0 root         (0) root         (0)     5149 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/execute_in_process.py
--rw-r--r--   0 root         (0) root         (0)     5426 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/execute_in_process_result.py
--rw-r--r--   0 root         (0) root         (0)     9183 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/execution_result.py
--rw-r--r--   0 root         (0) root         (0)     8544 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/host_mode.py
--rw-r--r--   0 root         (0) root         (0)    14451 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/job_backfill.py
--rw-r--r--   0 root         (0) root         (0)     6487 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/job_execution_result.py
--rw-r--r--   0 root         (0) root         (0)      998 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/memoization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.061473 dagster-1.3.5/dagster/_core/execution/plan/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/plan/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23031 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/plan/active.py
--rw-r--r--   0 root         (0) root         (0)     7279 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/plan/compute.py
--rw-r--r--   0 root         (0) root         (0)    12550 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/plan/compute_generator.py
--rw-r--r--   0 root         (0) root         (0)    16270 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/plan/execute_plan.py
--rw-r--r--   0 root         (0) root         (0)    27355 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/plan/execute_step.py
--rw-r--r--   0 root         (0) root         (0)    10000 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/plan/external_step.py
--rw-r--r--   0 root         (0) root         (0)     3664 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/plan/handle.py
--rw-r--r--   0 root         (0) root         (0)    37831 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/plan/inputs.py
--rw-r--r--   0 root         (0) root         (0)     1159 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/plan/local_external_step_main.py
--rw-r--r--   0 root         (0) root         (0)     5395 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/plan/objects.py
--rw-r--r--   0 root         (0) root         (0)     7057 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/plan/outputs.py
--rw-r--r--   0 root         (0) root         (0)    57790 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/plan/plan.py
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/plan/resume_retry.py
--rw-r--r--   0 root         (0) root         (0)    15616 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/plan/state.py
--rw-r--r--   0 root         (0) root         (0)    15920 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/plan/step.py
--rw-r--r--   0 root         (0) root         (0)     3796 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/plan/utils.py
--rw-r--r--   0 root         (0) root         (0)     1762 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/poll_compute_logs.py
--rw-r--r--   0 root         (0) root         (0)     8186 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/resolve_versions.py
--rw-r--r--   0 root         (0) root         (0)    19280 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/resources_init.py
--rw-r--r--   0 root         (0) root         (0)     2104 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/retries.py
--rw-r--r--   0 root         (0) root         (0)     1651 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/run_cancellation_thread.py
--rw-r--r--   0 root         (0) root         (0)    10329 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/stats.py
--rw-r--r--   0 root         (0) root         (0)     1125 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/tags.py
--rw-r--r--   0 root         (0) root         (0)     1172 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/validate_run_config.py
--rw-r--r--   0 root         (0) root         (0)     1282 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/watch_orphans.py
--rw-r--r--   0 root         (0) root         (0)     4233 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/execution/with_resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.065472 dagster-1.3.5/dagster/_core/executor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/executor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1265 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/executor/base.py
--rw-r--r--   0 root         (0) root         (0)     5990 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/executor/child_process_executor.py
--rw-r--r--   0 root         (0) root         (0)     2840 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/executor/in_process.py
--rw-r--r--   0 root         (0) root         (0)     1509 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/executor/init.py
--rw-r--r--   0 root         (0) root         (0)    15667 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/executor/multiprocess.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.065472 dagster-1.3.5/dagster/_core/executor/step_delegating/
--rw-r--r--   0 root         (0) root         (0)      247 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/executor/step_delegating/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14328 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/executor/step_delegating/step_delegating_executor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.065472 dagster-1.3.5/dagster/_core/executor/step_delegating/step_handler/
--rw-r--r--   0 root         (0) root         (0)      152 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/executor/step_delegating/step_handler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3078 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/executor/step_delegating/step_handler/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.065472 dagster-1.3.5/dagster/_core/host_representation/
--rw-r--r--   0 root         (0) root         (0)     2789 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/host_representation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33518 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/host_representation/code_location.py
--rw-r--r--   0 root         (0) root         (0)    32089 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/host_representation/external.py
--rw-r--r--   0 root         (0) root         (0)    70934 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/host_representation/external_data.py
--rw-r--r--   0 root         (0) root         (0)    11276 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/host_representation/grpc_server_registry.py
--rw-r--r--   0 root         (0) root         (0)     1487 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/host_representation/grpc_server_state_subscriber.py
--rw-r--r--   0 root         (0) root         (0)     4333 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/host_representation/handle.py
--rw-r--r--   0 root         (0) root         (0)     1581 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/host_representation/historical.py
--rw-r--r--   0 root         (0) root         (0)     4850 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/host_representation/job_index.py
--rw-r--r--   0 root         (0) root         (0)    17368 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/host_representation/origin.py
--rw-r--r--   0 root         (0) root         (0)     3610 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/host_representation/represented.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.065472 dagster-1.3.5/dagster/_core/instance/
--rw-r--r--   0 root         (0) root         (0)   103917 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/instance/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11650 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/instance/config.py
--rw-r--r--   0 root         (0) root         (0)    24318 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/instance/ref.py
--rw-r--r--   0 root         (0) root         (0)     4567 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/instance_for_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.065472 dagster-1.3.5/dagster/_core/launcher/
--rw-r--r--   0 root         (0) root         (0)      297 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3639 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/launcher/base.py
--rw-r--r--   0 root         (0) root         (0)     6629 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/launcher/default_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1586 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/launcher/sync_in_memory_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/libraries.py
--rw-r--r--   0 root         (0) root         (0)    17249 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1029 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/nux.py
--rw-r--r--   0 root         (0) root         (0)     3691 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/origin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.065472 dagster-1.3.5/dagster/_core/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      267 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2005 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/run_coordinator/base.py
--rw-r--r--   0 root         (0) root         (0)     1922 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/run_coordinator/default_run_coordinator.py
--rw-r--r--   0 root         (0) root         (0)    11030 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/run_coordinator/queued_run_coordinator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.065472 dagster-1.3.5/dagster/_core/scheduler/
--rw-r--r--   0 root         (0) root         (0)      534 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1241 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/scheduler/execution.py
--rw-r--r--   0 root         (0) root         (0)    21475 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/scheduler/instigation.py
--rw-r--r--   0 root         (0) root         (0)     9410 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/scheduler/scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.069472 dagster-1.3.5/dagster/_core/secrets/
--rw-r--r--   0 root         (0) root         (0)       51 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1777 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/secrets/env_file.py
--rw-r--r--   0 root         (0) root         (0)      388 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.069472 dagster-1.3.5/dagster/_core/selector/
--rw-r--r--   0 root         (0) root         (0)      295 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/selector/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18247 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/selector/subset_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.069472 dagster-1.3.5/dagster/_core/snap/
--rw-r--r--   0 root         (0) root         (0)     2815 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/snap/__init__.py
--rw-r--r--   0 root         (0) root         (0)      494 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/snap/config_types.py
--rw-r--r--   0 root         (0) root         (0)     3999 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/snap/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     9421 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/snap/dep_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    12099 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/snap/execution_plan_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    16654 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/snap/job_snapshot.py
--rw-r--r--   0 root         (0) root         (0)     4495 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/snap/mode.py
--rw-r--r--   0 root         (0) root         (0)    14452 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/snap/node.py
--rw-r--r--   0 root         (0) root         (0)     1917 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/snap/snap_to_yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.073473 dagster-1.3.5/dagster/_core/storage/
--rw-r--r--   0 root         (0) root         (0)     3057 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/DEVELOPING.md
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.077473 dagster-1.3.5/dagster/_core/storage/alembic/
--rw-r--r--   0 root         (0) root         (0)     6676 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/README.md
--rw-r--r--   0 root         (0) root         (0)      687 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      494 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.085472 dagster-1.3.5/dagster/_core/storage/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     3150 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/001_initial_1.py
--rw-r--r--   0 root         (0) root         (0)      311 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/001_initial_schedule.py
--rw-r--r--   0 root         (0) root         (0)     1353 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
--rw-r--r--   0 root         (0) root         (0)      598 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     2548 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
--rw-r--r--   0 root         (0) root         (0)     1405 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1405 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1729 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1729 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1146 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1124 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
--rw-r--r--   0 root         (0) root         (0)     1142 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
--rw-r--r--   0 root         (0) root         (0)      416 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      416 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      431 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      431 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     3926 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
--rw-r--r--   0 root         (0) root         (0)     3926 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      935 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      935 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      325 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/017_initial_mysql.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1569 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1569 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1031 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      530 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      634 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1892 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
--rw-r--r--   0 root         (0) root         (0)      957 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
--rw-r--r--   0 root         (0) root         (0)      498 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
--rw-r--r--   0 root         (0) root         (0)      428 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
--rw-r--r--   0 root         (0) root         (0)      426 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
--rw-r--r--   0 root         (0) root         (0)     2480 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
--rw-r--r--   0 root         (0) root         (0)     1176 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py
--rw-r--r--   0 root         (0) root         (0)     2062 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7204 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/asset_value_loader.py
--rw-r--r--   0 root         (0) root         (0)     1215 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/base_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.085472 dagster-1.3.5/dagster/_core/storage/branching/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/branching/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4304 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/branching/branching_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8736 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/captured_log_manager.py
--rw-r--r--   0 root         (0) root         (0)    16247 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/cloud_storage_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     9545 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1863 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/config.py
--rw-r--r--   0 root         (0) root         (0)      417 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/daemon_cursor.py
--rw-r--r--   0 root         (0) root         (0)    23596 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/dagster_run.py
--rw-r--r--   0 root         (0) root         (0)    11640 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/db_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.089472 dagster-1.3.5/dagster/_core/storage/event_log/
--rw-r--r--   0 root         (0) root         (0)      742 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/event_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14381 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/event_log/base.py
--rw-r--r--   0 root         (0) root         (0)     3630 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/event_log/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     7211 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/event_log/migration.py
--rw-r--r--   0 root         (0) root         (0)     7911 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/event_log/polling_event_watcher.py
--rw-r--r--   0 root         (0) root         (0)     5090 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/event_log/schema.py
--rw-r--r--   0 root         (0) root         (0)    78441 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/event_log/sql_event_log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.089472 dagster-1.3.5/dagster/_core/storage/event_log/sqlite/
--rw-r--r--   0 root         (0) root         (0)      200 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/event_log/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.089472 dagster-1.3.5/dagster/_core/storage/event_log/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)     1040 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     7408 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    18950 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    10912 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/file_manager.py
--rw-r--r--   0 root         (0) root         (0)    13217 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/fs_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8915 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/input_manager.py
--rw-r--r--   0 root         (0) root         (0)    10638 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/io_manager.py
--rw-r--r--   0 root         (0) root         (0)    27079 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/legacy_storage.py
--rw-r--r--   0 root         (0) root         (0)    17301 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/local_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)      876 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/mem_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     4293 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/memoizable_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.089472 dagster-1.3.5/dagster/_core/storage/migration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/migration/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14469 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/migration/utils.py
--rw-r--r--   0 root         (0) root         (0)     3186 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/noop_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     2361 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/output_manager.py
--rw-r--r--   0 root         (0) root         (0)    23189 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/partition_status_cache.py
--rw-r--r--   0 root         (0) root         (0)     2121 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/root.py
--rw-r--r--   0 root         (0) root         (0)     8509 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/root_input_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.089472 dagster-1.3.5/dagster/_core/storage/runs/
--rw-r--r--   0 root         (0) root         (0)      386 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15454 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/runs/base.py
--rw-r--r--   0 root         (0) root         (0)     2291 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/runs/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     8635 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/runs/migration.py
--rw-r--r--   0 root         (0) root         (0)     5982 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/runs/schema.py
--rw-r--r--   0 root         (0) root         (0)    46394 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/runs/sql_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.089472 dagster-1.3.5/dagster/_core/storage/runs/sqlite/
--rw-r--r--   0 root         (0) root         (0)       69 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/runs/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.089472 dagster-1.3.5/dagster/_core/storage/runs/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)     1040 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     6822 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.089472 dagster-1.3.5/dagster/_core/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)      272 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6256 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/schedules/base.py
--rw-r--r--   0 root         (0) root         (0)     4095 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/schedules/migration.py
--rw-r--r--   0 root         (0) root         (0)     3695 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/schedules/schema.py
--rw-r--r--   0 root         (0) root         (0)    22092 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/schedules/sql_schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.089472 dagster-1.3.5/dagster/_core/storage/schedules/sqlite/
--rw-r--r--   0 root         (0) root         (0)       84 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/schedules/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.089472 dagster-1.3.5/dagster/_core/storage/schedules/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)     1039 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     3664 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
--rw-r--r--   0 root         (0) root         (0)     7375 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/sql.py
--rw-r--r--   0 root         (0) root         (0)      926 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/sqlite.py
--rw-r--r--   0 root         (0) root         (0)     4863 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/sqlite_storage.py
--rw-r--r--   0 root         (0) root         (0)     3082 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/tags.py
--rw-r--r--   0 root         (0) root         (0)     1128 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/temp_file_manager.py
--rw-r--r--   0 root         (0) root         (0)    11346 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/storage/upath_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.089472 dagster-1.3.5/dagster/_core/system_config/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/system_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13981 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/system_config/composite_descent.py
--rw-r--r--   0 root         (0) root         (0)    14855 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/system_config/objects.py
--rw-r--r--   0 root         (0) root         (0)    27932 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     4824 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/telemetry_upload.py
--rw-r--r--   0 root         (0) root         (0)    18922 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.093473 dagster-1.3.5/dagster/_core/types/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3163 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/types/builtin_config_schemas.py
--rw-r--r--   0 root         (0) root         (0)     7298 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/types/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    35761 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/types/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)     3579 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/types/decorator.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/types/loadable_target_origin.py
--rw-r--r--   0 root         (0) root         (0)     1027 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/types/primitive_mapping.py
--rw-r--r--   0 root         (0) root         (0)     4881 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/types/python_dict.py
--rw-r--r--   0 root         (0) root         (0)     2836 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/types/python_set.py
--rw-r--r--   0 root         (0) root         (0)     3712 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/types/python_tuple.py
--rw-r--r--   0 root         (0) root         (0)     1772 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/types/transform_typing.py
--rw-r--r--   0 root         (0) root         (0)     1438 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/utility_ops.py
--rw-r--r--   0 root         (0) root         (0)     4003 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.093473 dagster-1.3.5/dagster/_core/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4722 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/workspace/autodiscovery.py
--rw-r--r--   0 root         (0) root         (0)     3478 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/workspace/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    26620 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/workspace/context.py
--rw-r--r--   0 root         (0) root         (0)    11881 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/workspace/load.py
--rw-r--r--   0 root         (0) root         (0)     4684 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/workspace/load_target.py
--rw-r--r--   0 root         (0) root         (0)     3952 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/workspace/permissions.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_core/workspace/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.093473 dagster-1.3.5/dagster/_daemon/
--rw-r--r--   0 root         (0) root         (0)     1930 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_daemon/__init__.py
--rw-r--r--   0 root         (0) root         (0)       30 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_daemon/__main__.py
--rw-r--r--   0 root         (0) root         (0)     5236 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_daemon/asset_daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.093473 dagster-1.3.5/dagster/_daemon/auto_run_reexecution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_daemon/auto_run_reexecution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6822 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
--rw-r--r--   0 root         (0) root         (0)     9123 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
--rw-r--r--   0 root         (0) root         (0)     1936 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_daemon/backfill.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.093473 dagster-1.3.5/dagster/_daemon/cli/
--rw-r--r--   0 root         (0) root         (0)     4399 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_daemon/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17726 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_daemon/controller.py
--rw-r--r--   0 root         (0) root         (0)    10457 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_daemon/daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.093473 dagster-1.3.5/dagster/_daemon/monitoring/
--rw-r--r--   0 root         (0) root         (0)      215 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_daemon/monitoring/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10032 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_daemon/monitoring/monitoring_daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.093473 dagster-1.3.5/dagster/_daemon/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      100 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_daemon/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16247 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
--rw-r--r--   0 root         (0) root         (0)    37645 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_daemon/sensor.py
--rw-r--r--   0 root         (0) root         (0)     2860 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_daemon/types.py
--rw-r--r--   0 root         (0) root         (0)     6639 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_daemon/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.093473 dagster-1.3.5/dagster/_experimental/
--rw-r--r--   0 root         (0) root         (0)      300 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_experimental/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.093473 dagster-1.3.5/dagster/_generate/
--rw-r--r--   0 root         (0) root         (0)      253 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2720 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/download.py
--rw-r--r--   0 root         (0) root         (0)     4805 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/generate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.025472 dagster-1.3.5/dagster/_generate/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.097473 dagster-1.3.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.097473 dagster-1.3.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)      175 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.097473 dagster-1.3.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)      137 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
--rw-r--r--   0 root         (0) root         (0)       43 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      285 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.097473 dagster-1.3.5/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)     1753 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.097473 dagster-1.3.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.097473 dagster-1.3.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
--rw-r--r--   0 root         (0) root         (0)      164 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.097473 dagster-1.3.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)       80 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       34 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      267 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.097473 dagster-1.3.5/dagster/_grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.097473 dagster-1.3.5/dagster/_grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      178 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28114 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_grpc/__generated__/api_pb2.py
--rw-r--r--   0 root         (0) root         (0)    38178 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_grpc/__generated__/api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2051 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)       89 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_grpc/__main__.py
--rw-r--r--   0 root         (0) root         (0)    18324 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     4202 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_grpc/compile.py
--rw-r--r--   0 root         (0) root         (0)    21967 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_grpc/impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.097473 dagster-1.3.5/dagster/_grpc/protos/
--rw-r--r--   0 root         (0) root         (0)     5394 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_grpc/protos/api.proto
--rw-r--r--   0 root         (0) root         (0)    51206 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_grpc/server.py
--rw-r--r--   0 root         (0) root         (0)     5301 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_grpc/server_watcher.py
--rw-r--r--   0 root         (0) root         (0)    26559 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_grpc/types.py
--rw-r--r--   0 root         (0) root         (0)     2323 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_grpc/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.097473 dagster-1.3.5/dagster/_legacy/
--rw-r--r--   0 root         (0) root         (0)      222 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_legacy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.097473 dagster-1.3.5/dagster/_loggers/
--rw-r--r--   0 root         (0) root         (0)     3781 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_loggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3269 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_module_alias_map.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.097473 dagster-1.3.5/dagster/_scheduler/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31790 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_scheduler/scheduler.py
--rw-r--r--   0 root         (0) root         (0)     1361 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_scheduler/stale.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.101472 dagster-1.3.5/dagster/_serdes/
--rw-r--r--   0 root         (0) root         (0)      629 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_serdes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8004 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_serdes/config_class.py
--rw-r--r--   0 root         (0) root         (0)      142 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_serdes/errors.py
--rw-r--r--   0 root         (0) root         (0)     7467 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_serdes/ipc.py
--rw-r--r--   0 root         (0) root         (0)    37613 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_serdes/serdes.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_serdes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.101472 dagster-1.3.5/dagster/_seven/
--rw-r--r--   0 root         (0) root         (0)     5496 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_seven/__init__.py
--rw-r--r--   0 root         (0) root         (0)      553 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_seven/abc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.101472 dagster-1.3.5/dagster/_seven/compat/
--rw-r--r--   0 root         (0) root         (0)      105 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_seven/compat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1160 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_seven/compat/pendulum.py
--rw-r--r--   0 root         (0) root         (0)      383 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_seven/json.py
--rw-r--r--   0 root         (0) root         (0)      354 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_seven/temp_dir.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.105472 dagster-1.3.5/dagster/_utils/
--rw-r--r--   0 root         (0) root         (0)    23319 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8741 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/alert.py
--rw-r--r--   0 root         (0) root         (0)     6965 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/backcompat.py
--rw-r--r--   0 root         (0) root         (0)     2250 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/backoff.py
--rw-r--r--   0 root         (0) root         (0)     4116 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/cached_method.py
--rw-r--r--   0 root         (0) root         (0)    24259 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/caching_instance_queryer.py
--rw-r--r--   0 root         (0) root         (0)     2563 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)     4094 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/error.py
--rw-r--r--   0 root         (0) root         (0)     1264 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/external.py
--rw-r--r--   0 root         (0) root         (0)      883 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/forked_pdb.py
--rw-r--r--   0 root         (0) root         (0)     2344 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/hosted_user_process.py
--rw-r--r--   0 root         (0) root         (0)     2796 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/indenting_printer.py
--rw-r--r--   0 root         (0) root         (0)      344 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/internal_init.py
--rw-r--r--   0 root         (0) root         (0)     3227 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/interrupts.py
--rw-r--r--   0 root         (0) root         (0)     9813 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/log.py
--rw-r--r--   0 root         (0) root         (0)     2313 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/merger.py
--rw-r--r--   0 root         (0) root         (0)     1507 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/net.py
--rw-r--r--   0 root         (0) root         (0)      208 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/partitions.py
--rw-r--r--   0 root         (0) root         (0)    12340 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/schedules.py
--rw-r--r--   0 root         (0) root         (0)     3289 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/tags.py
--rw-r--r--   0 root         (0) root         (0)     1820 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/temp_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.105472 dagster-1.3.5/dagster/_utils/test/
--rw-r--r--   0 root         (0) root         (0)    10412 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/test/hello_world_defs.py
--rw-r--r--   0 root         (0) root         (0)      214 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/test/hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     8622 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/test/mysql_instance.py
--rw-r--r--   0 root         (0) root         (0)      256 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/test/named_hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     9330 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/test/postgres_instance.py
--rw-r--r--   0 root         (0) root         (0)    26853 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/test/schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.105472 dagster-1.3.5/dagster/_utils/test/toys/
--rw-r--r--   0 root         (0) root         (0)       83 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/test/toys/__init__.py
--rw-r--r--   0 root         (0) root         (0)       84 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/test/toys/single_repository.py
--rw-r--r--   0 root         (0) root         (0)     2004 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/timing.py
--rw-r--r--   0 root         (0) root         (0)      170 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/types.py
--rw-r--r--   0 root         (0) root         (0)     3334 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/typing_api.py
--rw-r--r--   0 root         (0) root         (0)     4915 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/_utils/yaml_utils.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/py.typed
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 20:38:07.000000 dagster-1.3.5/dagster/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:38:25.029472 dagster-1.3.5/dagster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8790 2023-05-18 20:38:24.000000 dagster-1.3.5/dagster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    25105 2023-05-18 20:38:24.000000 dagster-1.3.5/dagster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 20:38:24.000000 dagster-1.3.5/dagster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       86 2023-05-18 20:38:24.000000 dagster-1.3.5/dagster.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     1309 2023-05-18 20:38:24.000000 dagster-1.3.5/dagster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-18 20:38:24.000000 dagster-1.3.5/dagster.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      154 2023-05-18 20:38:25.105472 dagster-1.3.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6440 2023-05-18 20:38:07.000000 dagster-1.3.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.351283 dagster-1.3.6/
+-rw-r--r--   0 root         (0) root         (0)      549 2023-05-25 17:16:49.000000 dagster-1.3.6/COPYING
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-05-25 17:16:49.000000 dagster-1.3.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      485 2023-05-25 17:16:49.000000 dagster-1.3.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8790 2023-05-25 17:17:08.351283 dagster-1.3.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7167 2023-05-25 17:16:49.000000 dagster-1.3.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.287283 dagster-1.3.6/dagster/
+-rw-r--r--   0 root         (0) root         (0)    26157 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     5456 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_annotations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.287283 dagster-1.3.6/dagster/_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      731 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_api/get_server_id.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_api/list_repositories.py
+-rw-r--r--   0 root         (0) root         (0)      531 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_api/notebook_data.py
+-rw-r--r--   0 root         (0) root         (0)     2882 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_api/snapshot_execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_api/snapshot_job.py
+-rw-r--r--   0 root         (0) root         (0)     5479 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_api/snapshot_partition.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_api/snapshot_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2727 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_api/snapshot_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     2901 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_api/snapshot_sensor.py
+-rw-r--r--   0 root         (0) root         (0)      478 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_builtins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.291283 dagster-1.3.6/dagster/_check/
+-rw-r--r--   0 root         (0) root         (0)     1352 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_check/README.md
+-rw-r--r--   0 root         (0) root         (0)    51637 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_check/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.291283 dagster-1.3.6/dagster/_cli/
+-rw-r--r--   0 root         (0) root         (0)     1182 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27241 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_cli/api.py
+-rw-r--r--   0 root         (0) root         (0)     8186 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_cli/asset.py
+-rw-r--r--   0 root         (0) root         (0)     7730 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_cli/code_server.py
+-rw-r--r--   0 root         (0) root         (0)     2300 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_cli/config_scaffolder.py
+-rw-r--r--   0 root         (0) root         (0)     3533 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_cli/debug.py
+-rw-r--r--   0 root         (0) root         (0)     5845 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_cli/dev.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_cli/instance.py
+-rw-r--r--   0 root         (0) root         (0)    29822 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_cli/job.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_cli/load_handle.py
+-rw-r--r--   0 root         (0) root         (0)     5852 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_cli/project.py
+-rw-r--r--   0 root         (0) root         (0)     5135 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_cli/run.py
+-rw-r--r--   0 root         (0) root         (0)    19909 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_cli/schedule.py
+-rw-r--r--   0 root         (0) root         (0)    15661 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_cli/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     1409 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.291283 dagster-1.3.6/dagster/_cli/workspace/
+-rw-r--r--   0 root         (0) root         (0)      180 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_cli/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28391 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_cli/workspace/cli_target.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.295283 dagster-1.3.6/dagster/_config/
+-rw-r--r--   0 root         (0) root         (0)     3186 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3403 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    15864 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/config_type.py
+-rw-r--r--   0 root         (0) root         (0)    19601 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1783 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/evaluate_value_result.py
+-rw-r--r--   0 root         (0) root         (0)    15269 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/field.py
+-rw-r--r--   0 root         (0) root         (0)    16880 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/field_utils.py
+-rw-r--r--   0 root         (0) root         (0)     9466 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/post_process.py
+-rw-r--r--   0 root         (0) root         (0)      855 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/primitive_mapping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.295283 dagster-1.3.6/dagster/_config/pythonic_config/
+-rw-r--r--   0 root         (0) root         (0)    71109 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/pythonic_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/pythonic_config/attach_other_object_to_context.py
+-rw-r--r--   0 root         (0) root         (0)     6217 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/pythonic_config/typing_utils.py
+-rw-r--r--   0 root         (0) root         (0)      577 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/pythonic_config/utils.py
+-rw-r--r--   0 root         (0) root         (0)    12143 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/snap.py
+-rw-r--r--   0 root         (0) root         (0)     3267 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/source.py
+-rw-r--r--   0 root         (0) root         (0)     3528 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/stack.py
+-rw-r--r--   0 root         (0) root         (0)     7772 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/traversal_context.py
+-rw-r--r--   0 root         (0) root         (0)     4167 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/type_printer.py
+-rw-r--r--   0 root         (0) root         (0)    17162 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_config/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.295283 dagster-1.3.6/dagster/_core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      994 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/assets.py
+-rw-r--r--   0 root         (0) root         (0)    13645 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/code_pointer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.295283 dagster-1.3.6/dagster/_core/container_context/
+-rw-r--r--   0 root         (0) root         (0)      184 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/container_context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/container_context/config.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/debug.py
+-rw-r--r--   0 root         (0) root         (0)     3005 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/decorator_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.303283 dagster-1.3.6/dagster/_core/definitions/
+-rw-r--r--   0 root         (0) root         (0)     7626 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30229 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)    10704 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/asset_graph_subset.py
+-rw-r--r--   0 root         (0) root         (0)     3816 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/asset_in.py
+-rw-r--r--   0 root         (0) root         (0)    36842 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/asset_layer.py
+-rw-r--r--   0 root         (0) root         (0)     5685 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/asset_out.py
+-rw-r--r--   0 root         (0) root         (0)    58294 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/asset_reconciliation_sensor.py
+-rw-r--r--   0 root         (0) root         (0)    18474 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/asset_selection.py
+-rw-r--r--   0 root         (0) root         (0)     7164 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    64821 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/assets.py
+-rw-r--r--   0 root         (0) root         (0)    24005 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/assets_job.py
+-rw-r--r--   0 root         (0) root         (0)     2806 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/auto_materialize_condition.py
+-rw-r--r--   0 root         (0) root         (0)     5297 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16105 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/cacheable_assets.py
+-rw-r--r--   0 root         (0) root         (0)    45671 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/composition.py
+-rw-r--r--   0 root         (0) root         (0)     4287 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/config.py
+-rw-r--r--   0 root         (0) root         (0)    10845 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/configurable.py
+-rw-r--r--   0 root         (0) root         (0)    20795 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/data_time.py
+-rw-r--r--   0 root         (0) root         (0)    17905 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/data_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.307283 dagster-1.3.6/dagster/_core/definitions/decorators/
+-rw-r--r--   0 root         (0) root         (0)      620 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43205 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/decorators/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4915 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/decorators/config_mapping_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     8250 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/decorators/graph_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     9444 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/decorators/hook_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    10676 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/decorators/job_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    17845 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/decorators/op_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    14396 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/decorators/repository_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     8656 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/decorators/schedule_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    11936 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/decorators/sensor_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     6591 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/decorators/source_asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     5275 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/definition_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    20546 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/definitions_class.py
+-rw-r--r--   0 root         (0) root         (0)    39988 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/dependency.py
+-rw-r--r--   0 root         (0) root         (0)    31576 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/events.py
+-rw-r--r--   0 root         (0) root         (0)    21013 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/executor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    10548 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/external_asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)     8010 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16195 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/freshness_policy_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    44740 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/graph_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6546 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/hook_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1515 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/hook_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3205 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/inference.py
+-rw-r--r--   0 root         (0) root         (0)    22898 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/input.py
+-rw-r--r--   0 root         (0) root         (0)     5386 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/instigation_logger.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/job_base.py
+-rw-r--r--   0 root         (0) root         (0)    51157 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/job_definition.py
+-rw-r--r--   0 root         (0) root         (0)    20308 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/load_assets_from_modules.py
+-rw-r--r--   0 root         (0) root         (0)     6845 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/logger_definition.py
+-rw-r--r--   0 root         (0) root         (0)      636 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/logger_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     8841 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/materialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.307283 dagster-1.3.6/dagster/_core/definitions/metadata/
+-rw-r--r--   0 root         (0) root         (0)    32319 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8557 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/metadata/table.py
+-rw-r--r--   0 root         (0) root         (0)    56090 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/multi_asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    20758 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/multi_dimensional_partitions.py
+-rw-r--r--   0 root         (0) root         (0)       82 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/no_step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)    11927 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/node_container.py
+-rw-r--r--   0 root         (0) root         (0)     8041 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/node_definition.py
+-rw-r--r--   0 root         (0) root         (0)     2867 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/observe.py
+-rw-r--r--   0 root         (0) root         (0)    22629 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/op_definition.py
+-rw-r--r--   0 root         (0) root         (0)    19256 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/op_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     7509 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/op_selection.py
+-rw-r--r--   0 root         (0) root         (0)    18908 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/output.py
+-rw-r--r--   0 root         (0) root         (0)    39032 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/partition.py
+-rw-r--r--   0 root         (0) root         (0)      196 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/partition_key_range.py
+-rw-r--r--   0 root         (0) root         (0)    47274 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     8811 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/partitioned_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     3779 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/policy.py
+-rw-r--r--   0 root         (0) root         (0)    27231 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/reconstruct.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.307283 dagster-1.3.6/dagster/_core/definitions/repository_definition/
+-rw-r--r--   0 root         (0) root         (0)      654 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/repository_definition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6670 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/repository_definition/caching_index.py
+-rw-r--r--   0 root         (0) root         (0)    18856 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/repository_definition/repository_data.py
+-rw-r--r--   0 root         (0) root         (0)    17401 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/repository_definition/repository_data_builder.py
+-rw-r--r--   0 root         (0) root         (0)    16917 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/repository_definition/repository_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/repository_definition/valid_definitions.py
+-rw-r--r--   0 root         (0) root         (0)     5108 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/resolved_asset_deps.py
+-rw-r--r--   0 root         (0) root         (0)     1336 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/resource_annotation.py
+-rw-r--r--   0 root         (0) root         (0)    16162 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/resource_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5398 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/resource_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     7806 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/resource_requirement.py
+-rw-r--r--   0 root         (0) root         (0)    24105 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1445 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    15824 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/run_request.py
+-rw-r--r--   0 root         (0) root         (0)    38400 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/run_status_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    37556 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/schedule_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5189 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/scoped_resources_builder.py
+-rw-r--r--   0 root         (0) root         (0)    10837 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/selector.py
+-rw-r--r--   0 root         (0) root         (0)    46882 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    14148 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/source_asset.py
+-rw-r--r--   0 root         (0) root         (0)     2298 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/target.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/test_op_definition.py
+-rw-r--r--   0 root         (0) root         (0)    12374 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/time_window_partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)    76525 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/time_window_partitions.py
+-rw-r--r--   0 root         (0) root         (0)    15645 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/unresolved_asset_job_definition.py
+-rw-r--r--   0 root         (0) root         (0)     7992 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2930 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/definitions/version_strategy.py
+-rw-r--r--   0 root         (0) root         (0)    25453 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/errors.py
+-rw-r--r--   0 root         (0) root         (0)     6241 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/event_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.307283 dagster-1.3.6/dagster/_core/events/
+-rw-r--r--   0 root         (0) root         (0)    64981 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/events/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7783 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/events/log.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/events/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.311283 dagster-1.3.6/dagster/_core/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38315 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/api.py
+-rw-r--r--   0 root         (0) root         (0)    30249 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/asset_backfill.py
+-rw-r--r--   0 root         (0) root         (0)    14476 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6487 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/build_resources.py
+-rw-r--r--   0 root         (0) root         (0)      224 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/bulk_actions.py
+-rw-r--r--   0 root         (0) root         (0)     5587 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/compute_logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.311283 dagster-1.3.6/dagster/_core/execution/context/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21992 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/context/compute.py
+-rw-r--r--   0 root         (0) root         (0)    15991 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/context/hook.py
+-rw-r--r--   0 root         (0) root         (0)     9369 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/context/init.py
+-rw-r--r--   0 root         (0) root         (0)    26845 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/context/input.py
+-rw-r--r--   0 root         (0) root         (0)    27417 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/context/invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3164 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/context/logger.py
+-rw-r--r--   0 root         (0) root         (0)    33974 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/context/output.py
+-rw-r--r--   0 root         (0) root         (0)    44193 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/context/system.py
+-rw-r--r--   0 root         (0) root         (0)    18501 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/context_creation_job.py
+-rw-r--r--   0 root         (0) root         (0)     5149 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/execute_in_process.py
+-rw-r--r--   0 root         (0) root         (0)     5426 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/execute_in_process_result.py
+-rw-r--r--   0 root         (0) root         (0)     9183 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/execution_result.py
+-rw-r--r--   0 root         (0) root         (0)     8544 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/host_mode.py
+-rw-r--r--   0 root         (0) root         (0)    14451 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/job_backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6487 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/job_execution_result.py
+-rw-r--r--   0 root         (0) root         (0)      998 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/memoization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.315283 dagster-1.3.6/dagster/_core/execution/plan/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/plan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23031 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/plan/active.py
+-rw-r--r--   0 root         (0) root         (0)     7279 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/plan/compute.py
+-rw-r--r--   0 root         (0) root         (0)    12550 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/plan/compute_generator.py
+-rw-r--r--   0 root         (0) root         (0)    16270 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/plan/execute_plan.py
+-rw-r--r--   0 root         (0) root         (0)    27355 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/plan/execute_step.py
+-rw-r--r--   0 root         (0) root         (0)    10000 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/plan/external_step.py
+-rw-r--r--   0 root         (0) root         (0)     3664 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/plan/handle.py
+-rw-r--r--   0 root         (0) root         (0)    37831 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/plan/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     1159 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/plan/local_external_step_main.py
+-rw-r--r--   0 root         (0) root         (0)     5395 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/plan/objects.py
+-rw-r--r--   0 root         (0) root         (0)     7057 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/plan/outputs.py
+-rw-r--r--   0 root         (0) root         (0)    57790 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/plan/plan.py
+-rw-r--r--   0 root         (0) root         (0)      114 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/plan/resume_retry.py
+-rw-r--r--   0 root         (0) root         (0)    15616 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/plan/state.py
+-rw-r--r--   0 root         (0) root         (0)    15920 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/plan/step.py
+-rw-r--r--   0 root         (0) root         (0)     3796 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/plan/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/poll_compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)     8186 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/resolve_versions.py
+-rw-r--r--   0 root         (0) root         (0)    19280 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/resources_init.py
+-rw-r--r--   0 root         (0) root         (0)     2104 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/retries.py
+-rw-r--r--   0 root         (0) root         (0)     1651 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/run_cancellation_thread.py
+-rw-r--r--   0 root         (0) root         (0)    10329 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/stats.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1172 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/validate_run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/watch_orphans.py
+-rw-r--r--   0 root         (0) root         (0)     4233 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/execution/with_resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.315283 dagster-1.3.6/dagster/_core/executor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/executor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/executor/base.py
+-rw-r--r--   0 root         (0) root         (0)     5990 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/executor/child_process_executor.py
+-rw-r--r--   0 root         (0) root         (0)     2840 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/executor/in_process.py
+-rw-r--r--   0 root         (0) root         (0)     1509 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/executor/init.py
+-rw-r--r--   0 root         (0) root         (0)    15667 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/executor/multiprocess.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.315283 dagster-1.3.6/dagster/_core/executor/step_delegating/
+-rw-r--r--   0 root         (0) root         (0)      247 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/executor/step_delegating/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14328 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/executor/step_delegating/step_delegating_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.315283 dagster-1.3.6/dagster/_core/executor/step_delegating/step_handler/
+-rw-r--r--   0 root         (0) root         (0)      152 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/executor/step_delegating/step_handler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/executor/step_delegating/step_handler/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.315283 dagster-1.3.6/dagster/_core/host_representation/
+-rw-r--r--   0 root         (0) root         (0)     2789 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/host_representation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33518 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/host_representation/code_location.py
+-rw-r--r--   0 root         (0) root         (0)    32089 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/host_representation/external.py
+-rw-r--r--   0 root         (0) root         (0)    70934 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/host_representation/external_data.py
+-rw-r--r--   0 root         (0) root         (0)    12283 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/host_representation/grpc_server_registry.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/host_representation/grpc_server_state_subscriber.py
+-rw-r--r--   0 root         (0) root         (0)     4333 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/host_representation/handle.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/host_representation/historical.py
+-rw-r--r--   0 root         (0) root         (0)     4850 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/host_representation/job_index.py
+-rw-r--r--   0 root         (0) root         (0)    19051 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/host_representation/origin.py
+-rw-r--r--   0 root         (0) root         (0)     3610 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/host_representation/represented.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.315283 dagster-1.3.6/dagster/_core/instance/
+-rw-r--r--   0 root         (0) root         (0)   104144 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/instance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12808 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/instance/config.py
+-rw-r--r--   0 root         (0) root         (0)    24318 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/instance/ref.py
+-rw-r--r--   0 root         (0) root         (0)     4567 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/instance_for_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.319283 dagster-1.3.6/dagster/_core/launcher/
+-rw-r--r--   0 root         (0) root         (0)      297 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3639 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/launcher/base.py
+-rw-r--r--   0 root         (0) root         (0)     6808 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/launcher/default_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1586 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/launcher/sync_in_memory_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/libraries.py
+-rw-r--r--   0 root         (0) root         (0)    17249 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/nux.py
+-rw-r--r--   0 root         (0) root         (0)     3691 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/origin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.319283 dagster-1.3.6/dagster/_core/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      267 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2005 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/run_coordinator/base.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/run_coordinator/default_run_coordinator.py
+-rw-r--r--   0 root         (0) root         (0)    11030 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/run_coordinator/queued_run_coordinator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.319283 dagster-1.3.6/dagster/_core/scheduler/
+-rw-r--r--   0 root         (0) root         (0)      534 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/scheduler/execution.py
+-rw-r--r--   0 root         (0) root         (0)    21903 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/scheduler/instigation.py
+-rw-r--r--   0 root         (0) root         (0)     9410 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/scheduler/scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.319283 dagster-1.3.6/dagster/_core/secrets/
+-rw-r--r--   0 root         (0) root         (0)       51 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1777 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/secrets/env_file.py
+-rw-r--r--   0 root         (0) root         (0)      388 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.319283 dagster-1.3.6/dagster/_core/selector/
+-rw-r--r--   0 root         (0) root         (0)      295 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/selector/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18247 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/selector/subset_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.319283 dagster-1.3.6/dagster/_core/snap/
+-rw-r--r--   0 root         (0) root         (0)     2815 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/snap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      494 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/snap/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     3999 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/snap/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     9421 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/snap/dep_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    12099 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/snap/execution_plan_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    16654 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/snap/job_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     4495 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/snap/mode.py
+-rw-r--r--   0 root         (0) root         (0)    14452 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/snap/node.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/snap/snap_to_yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.323283 dagster-1.3.6/dagster/_core/storage/
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/DEVELOPING.md
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.323283 dagster-1.3.6/dagster/_core/storage/alembic/
+-rw-r--r--   0 root         (0) root         (0)     6676 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/README.md
+-rw-r--r--   0 root         (0) root         (0)      687 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      494 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.331283 dagster-1.3.6/dagster/_core/storage/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     3150 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/001_initial_1.py
+-rw-r--r--   0 root         (0) root         (0)      311 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/001_initial_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     1353 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      598 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
+-rw-r--r--   0 root         (0) root         (0)      416 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      416 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      431 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      431 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     3926 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     3926 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      935 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      935 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      325 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/017_initial_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1569 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1569 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      530 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      634 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
+-rw-r--r--   0 root         (0) root         (0)      957 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
+-rw-r--r--   0 root         (0) root         (0)      498 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
+-rw-r--r--   0 root         (0) root         (0)      428 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
+-rw-r--r--   0 root         (0) root         (0)      426 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
+-rw-r--r--   0 root         (0) root         (0)     2480 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
+-rw-r--r--   0 root         (0) root         (0)     1176 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7204 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/asset_value_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1215 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/base_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.331283 dagster-1.3.6/dagster/_core/storage/branching/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/branching/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4304 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/branching/branching_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8736 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/captured_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)    16247 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/cloud_storage_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     9545 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/config.py
+-rw-r--r--   0 root         (0) root         (0)      417 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/daemon_cursor.py
+-rw-r--r--   0 root         (0) root         (0)    23596 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/dagster_run.py
+-rw-r--r--   0 root         (0) root         (0)    11640 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/db_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.331283 dagster-1.3.6/dagster/_core/storage/event_log/
+-rw-r--r--   0 root         (0) root         (0)      742 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/event_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14381 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/event_log/base.py
+-rw-r--r--   0 root         (0) root         (0)     3630 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/event_log/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     7211 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/event_log/migration.py
+-rw-r--r--   0 root         (0) root         (0)     7911 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/event_log/polling_event_watcher.py
+-rw-r--r--   0 root         (0) root         (0)     5090 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/event_log/schema.py
+-rw-r--r--   0 root         (0) root         (0)    78441 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/event_log/sql_event_log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.331283 dagster-1.3.6/dagster/_core/storage/event_log/sqlite/
+-rw-r--r--   0 root         (0) root         (0)      200 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/event_log/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.335283 dagster-1.3.6/dagster/_core/storage/event_log/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     7408 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    18950 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    10912 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    13217 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/fs_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8915 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/input_manager.py
+-rw-r--r--   0 root         (0) root         (0)    10638 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)    27079 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/legacy_storage.py
+-rw-r--r--   0 root         (0) root         (0)    17301 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/local_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)      876 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/mem_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4293 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/memoizable_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.335283 dagster-1.3.6/dagster/_core/storage/migration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/migration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14469 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/migration/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3186 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/noop_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/output_manager.py
+-rw-r--r--   0 root         (0) root         (0)    23189 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/partition_status_cache.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/root.py
+-rw-r--r--   0 root         (0) root         (0)     8509 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/root_input_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.335283 dagster-1.3.6/dagster/_core/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)      386 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15454 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/runs/base.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/runs/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     8635 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/runs/migration.py
+-rw-r--r--   0 root         (0) root         (0)     5982 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/runs/schema.py
+-rw-r--r--   0 root         (0) root         (0)    46394 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/runs/sql_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.335283 dagster-1.3.6/dagster/_core/storage/runs/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       69 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/runs/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.335283 dagster-1.3.6/dagster/_core/storage/runs/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     6822 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.335283 dagster-1.3.6/dagster/_core/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)      272 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6358 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/schedules/base.py
+-rw-r--r--   0 root         (0) root         (0)     4095 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/schedules/migration.py
+-rw-r--r--   0 root         (0) root         (0)     3710 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/schedules/schema.py
+-rw-r--r--   0 root         (0) root         (0)    22541 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/schedules/sql_schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.335283 dagster-1.3.6/dagster/_core/storage/schedules/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       84 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/schedules/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.335283 dagster-1.3.6/dagster/_core/storage/schedules/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     3664 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
+-rw-r--r--   0 root         (0) root         (0)     7375 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/sql.py
+-rw-r--r--   0 root         (0) root         (0)      926 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     4863 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/sqlite_storage.py
+-rw-r--r--   0 root         (0) root         (0)     3082 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/temp_file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    11346 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/storage/upath_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.335283 dagster-1.3.6/dagster/_core/system_config/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/system_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13981 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/system_config/composite_descent.py
+-rw-r--r--   0 root         (0) root         (0)    14855 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/system_config/objects.py
+-rw-r--r--   0 root         (0) root         (0)    27932 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     4824 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/telemetry_upload.py
+-rw-r--r--   0 root         (0) root         (0)    19369 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.339283 dagster-1.3.6/dagster/_core/types/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3163 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/types/builtin_config_schemas.py
+-rw-r--r--   0 root         (0) root         (0)     7298 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/types/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    35761 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/types/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)     3579 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/types/decorator.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/types/loadable_target_origin.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/types/primitive_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     4881 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/types/python_dict.py
+-rw-r--r--   0 root         (0) root         (0)     2836 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/types/python_set.py
+-rw-r--r--   0 root         (0) root         (0)     3712 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/types/python_tuple.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/types/transform_typing.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/utility_ops.py
+-rw-r--r--   0 root         (0) root         (0)     4003 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.339283 dagster-1.3.6/dagster/_core/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4722 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/workspace/autodiscovery.py
+-rw-r--r--   0 root         (0) root         (0)     3478 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/workspace/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    27515 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/workspace/context.py
+-rw-r--r--   0 root         (0) root         (0)    11881 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/workspace/load.py
+-rw-r--r--   0 root         (0) root         (0)     4684 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/workspace/load_target.py
+-rw-r--r--   0 root         (0) root         (0)     3952 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/workspace/permissions.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_core/workspace/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.339283 dagster-1.3.6/dagster/_daemon/
+-rw-r--r--   0 root         (0) root         (0)     1930 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_daemon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       30 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_daemon/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     5246 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_daemon/asset_daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.339283 dagster-1.3.6/dagster/_daemon/auto_run_reexecution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_daemon/auto_run_reexecution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6822 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
+-rw-r--r--   0 root         (0) root         (0)     9123 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
+-rw-r--r--   0 root         (0) root         (0)     1936 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_daemon/backfill.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.339283 dagster-1.3.6/dagster/_daemon/cli/
+-rw-r--r--   0 root         (0) root         (0)     4399 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_daemon/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17838 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_daemon/controller.py
+-rw-r--r--   0 root         (0) root         (0)    10457 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_daemon/daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.339283 dagster-1.3.6/dagster/_daemon/monitoring/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_daemon/monitoring/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10032 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_daemon/monitoring/monitoring_daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.343284 dagster-1.3.6/dagster/_daemon/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      100 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_daemon/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16247 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
+-rw-r--r--   0 root         (0) root         (0)    39799 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_daemon/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     2860 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_daemon/types.py
+-rw-r--r--   0 root         (0) root         (0)     6639 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_daemon/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.343284 dagster-1.3.6/dagster/_experimental/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_experimental/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.343284 dagster-1.3.6/dagster/_generate/
+-rw-r--r--   0 root         (0) root         (0)      253 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2720 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/download.py
+-rw-r--r--   0 root         (0) root         (0)     4805 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/generate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.283283 dagster-1.3.6/dagster/_generate/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.343284 dagster-1.3.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.343284 dagster-1.3.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)      175 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.343284 dagster-1.3.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)      137 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
+-rw-r--r--   0 root         (0) root         (0)       43 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      285 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.343284 dagster-1.3.6/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)     1753 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.343284 dagster-1.3.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.343284 dagster-1.3.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
+-rw-r--r--   0 root         (0) root         (0)      164 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.343284 dagster-1.3.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)       80 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       34 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      267 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.347283 dagster-1.3.6/dagster/_grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.347283 dagster-1.3.6/dagster/_grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      178 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29251 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_grpc/__generated__/api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    39700 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_grpc/__generated__/api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2051 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       89 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_grpc/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    18451 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     4202 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_grpc/compile.py
+-rw-r--r--   0 root         (0) root         (0)    21967 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_grpc/impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.347283 dagster-1.3.6/dagster/_grpc/protos/
+-rw-r--r--   0 root         (0) root         (0)     5551 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_grpc/protos/api.proto
+-rw-r--r--   0 root         (0) root         (0)    12415 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_grpc/proxy_server.py
+-rw-r--r--   0 root         (0) root         (0)    51587 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_grpc/server.py
+-rw-r--r--   0 root         (0) root         (0)     5301 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_grpc/server_watcher.py
+-rw-r--r--   0 root         (0) root         (0)    26559 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_grpc/types.py
+-rw-r--r--   0 root         (0) root         (0)     2323 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_grpc/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.347283 dagster-1.3.6/dagster/_legacy/
+-rw-r--r--   0 root         (0) root         (0)      222 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_legacy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.347283 dagster-1.3.6/dagster/_loggers/
+-rw-r--r--   0 root         (0) root         (0)     3781 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_loggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_module_alias_map.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.347283 dagster-1.3.6/dagster/_scheduler/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34303 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_scheduler/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_scheduler/stale.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.347283 dagster-1.3.6/dagster/_serdes/
+-rw-r--r--   0 root         (0) root         (0)      629 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_serdes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8004 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_serdes/config_class.py
+-rw-r--r--   0 root         (0) root         (0)      142 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_serdes/errors.py
+-rw-r--r--   0 root         (0) root         (0)     7467 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_serdes/ipc.py
+-rw-r--r--   0 root         (0) root         (0)    37613 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_serdes/serdes.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_serdes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.347283 dagster-1.3.6/dagster/_seven/
+-rw-r--r--   0 root         (0) root         (0)     5496 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_seven/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      553 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_seven/abc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.347283 dagster-1.3.6/dagster/_seven/compat/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_seven/compat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_seven/compat/pendulum.py
+-rw-r--r--   0 root         (0) root         (0)      383 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_seven/json.py
+-rw-r--r--   0 root         (0) root         (0)      354 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_seven/temp_dir.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.351283 dagster-1.3.6/dagster/_utils/
+-rw-r--r--   0 root         (0) root         (0)    23319 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8741 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/alert.py
+-rw-r--r--   0 root         (0) root         (0)     6965 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/backcompat.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/backoff.py
+-rw-r--r--   0 root         (0) root         (0)     4116 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/cached_method.py
+-rw-r--r--   0 root         (0) root         (0)    24259 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/caching_instance_queryer.py
+-rw-r--r--   0 root         (0) root         (0)     2563 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)     4094 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/error.py
+-rw-r--r--   0 root         (0) root         (0)     1264 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/external.py
+-rw-r--r--   0 root         (0) root         (0)      883 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/forked_pdb.py
+-rw-r--r--   0 root         (0) root         (0)     2344 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/hosted_user_process.py
+-rw-r--r--   0 root         (0) root         (0)     2796 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/indenting_printer.py
+-rw-r--r--   0 root         (0) root         (0)      344 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/internal_init.py
+-rw-r--r--   0 root         (0) root         (0)     3227 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/interrupts.py
+-rw-r--r--   0 root         (0) root         (0)     9813 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/log.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/merger.py
+-rw-r--r--   0 root         (0) root         (0)     1507 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/net.py
+-rw-r--r--   0 root         (0) root         (0)      208 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/partitions.py
+-rw-r--r--   0 root         (0) root         (0)    12340 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/schedules.py
+-rw-r--r--   0 root         (0) root         (0)     3289 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/temp_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.351283 dagster-1.3.6/dagster/_utils/test/
+-rw-r--r--   0 root         (0) root         (0)    10412 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/test/hello_world_defs.py
+-rw-r--r--   0 root         (0) root         (0)      214 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/test/hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     8622 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/test/mysql_instance.py
+-rw-r--r--   0 root         (0) root         (0)      256 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/test/named_hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     9330 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/test/postgres_instance.py
+-rw-r--r--   0 root         (0) root         (0)    28864 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/test/schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.351283 dagster-1.3.6/dagster/_utils/test/toys/
+-rw-r--r--   0 root         (0) root         (0)       83 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/test/toys/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       84 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/test/toys/single_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/timing.py
+-rw-r--r--   0 root         (0) root         (0)      170 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/types.py
+-rw-r--r--   0 root         (0) root         (0)     3334 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/typing_api.py
+-rw-r--r--   0 root         (0) root         (0)     4915 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/_utils/yaml_utils.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/py.typed
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-25 17:16:49.000000 dagster-1.3.6/dagster/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:17:08.287283 dagster-1.3.6/dagster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8790 2023-05-25 17:17:08.000000 dagster-1.3.6/dagster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    25163 2023-05-25 17:17:08.000000 dagster-1.3.6/dagster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 17:17:08.000000 dagster-1.3.6/dagster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2023-05-25 17:17:08.000000 dagster-1.3.6/dagster.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1317 2023-05-25 17:17:08.000000 dagster-1.3.6/dagster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-25 17:17:08.000000 dagster-1.3.6/dagster.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2023-05-25 17:17:08.355284 dagster-1.3.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6509 2023-05-25 17:16:50.000000 dagster-1.3.6/setup.py
```

### Comparing `dagster-1.3.5/COPYING` & `dagster-1.3.6/COPYING`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/LICENSE` & `dagster-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/PKG-INFO` & `dagster-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.3.5
+Version: 1.3.6
 Summary: The data orchestration platform built for productivity.
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Changelog, https://github.com/dagster-io/dagster/releases
```

### Comparing `dagster-1.3.5/README.md` & `dagster-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/__init__.py` & `dagster-1.3.6/dagster/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_annotations.py` & `dagster-1.3.6/dagster/_annotations.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_api/get_server_id.py` & `dagster-1.3.6/dagster/_api/get_server_id.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_api/list_repositories.py` & `dagster-1.3.6/dagster/_api/list_repositories.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_api/notebook_data.py` & `dagster-1.3.6/dagster/_api/notebook_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_api/snapshot_execution_plan.py` & `dagster-1.3.6/dagster/_api/snapshot_execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_api/snapshot_job.py` & `dagster-1.3.6/dagster/_api/snapshot_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_api/snapshot_partition.py` & `dagster-1.3.6/dagster/_api/snapshot_partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_api/snapshot_repository.py` & `dagster-1.3.6/dagster/_api/snapshot_repository.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_api/snapshot_schedule.py` & `dagster-1.3.6/dagster/_api/snapshot_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_api/snapshot_sensor.py` & `dagster-1.3.6/dagster/_api/snapshot_sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_check/README.md` & `dagster-1.3.6/dagster/_check/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_check/__init__.py` & `dagster-1.3.6/dagster/_check/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_cli/__init__.py` & `dagster-1.3.6/dagster/_cli/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import click
 
 from ..version import __version__
 from .api import api_cli
 from .asset import asset_cli
+from .code_server import code_server_cli
 from .debug import debug_cli
 from .dev import dev_command
 from .instance import instance_cli
 from .job import job_cli
 from .project import project_cli
 from .run import run_cli
 from .schedule import schedule_cli
@@ -21,14 +22,15 @@
         "instance": instance_cli,
         "schedule": schedule_cli,
         "sensor": sensor_cli,
         "asset": asset_cli,
         "debug": debug_cli,
         "project": project_cli,
         "dev": dev_command,
+        "code-server": code_server_cli,
     }
 
     @click.group(
         commands=commands,
         context_settings={"max_content_width": 120, "help_option_names": ["-h", "--help"]},
     )
     @click.version_option(__version__, "--version", "-v")
```

### Comparing `dagster-1.3.5/dagster/_cli/api.py` & `dagster-1.3.6/dagster/_cli/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,23 +26,22 @@
 from dagster._core.origin import (
     DEFAULT_DAGSTER_ENTRY_POINT,
     JobPythonOrigin,
     get_python_environment_entry_point,
 )
 from dagster._core.storage.dagster_run import DagsterRun
 from dagster._core.types.loadable_target_origin import LoadableTargetOrigin
-from dagster._core.utils import coerce_valid_log_level
 from dagster._grpc import DagsterGrpcClient, DagsterGrpcServer
 from dagster._grpc.impl import core_execute_run
 from dagster._grpc.server import DagsterApiServer
 from dagster._grpc.types import ExecuteRunArgs, ExecuteStepArgs, ResumeRunArgs
 from dagster._serdes import deserialize_value, serialize_value
 from dagster._utils.error import serializable_error_info_from_exc_info
 from dagster._utils.hosted_user_process import recon_job_from_origin
-from dagster._utils.interrupts import capture_interrupts
+from dagster._utils.interrupts import capture_interrupts, setup_interrupt_handlers
 from dagster._utils.log import configure_loggers
 
 
 @click.group(name="api", hidden=True)
 def api_cli():
     """[INTERNAL] These commands are intended to support internal use cases. Users should generally
     not invoke these commands interactively.
@@ -567,18 +566,19 @@
     help=(
         "[INTERNAL] This option should generally not be used by users. Override the system "
         "timezone for tests."
     ),
 )
 @click.option(
     "--log-level",
-    type=click.STRING,
+    type=click.Choice(["critical", "error", "warning", "info", "debug"], case_sensitive=False),
+    show_default=True,
     required=False,
-    default="INFO",
-    help="Level at which to log output from the gRPC server process",
+    default="info",
+    help="Level at which to log output from the code server process",
 )
 @click.option(
     "--container-image",
     type=click.STRING,
     required=False,
     help="Container image to use to run code from this server.",
     envvar="DAGSTER_CONTAINER_IMAGE",
@@ -649,16 +649,18 @@
     if seven.IS_WINDOWS and port is None:
         raise click.UsageError(
             "You must pass a valid --port/-p on Windows: --socket/-s not supported."
         )
     if not (port or socket and not (port and socket)):
         raise click.UsageError("You must pass one and only one of --port/-p or --socket/-s.")
 
-    configure_loggers(log_level=coerce_valid_log_level(log_level))
-    logger = logging.getLogger("dagster")
+    setup_interrupt_handlers()
+
+    configure_loggers(log_level=log_level.upper())
+    logger = logging.getLogger("dagster.code_server")
 
     container_image = container_image or os.getenv("DAGSTER_CURRENT_IMAGE")
 
     loadable_target_origin = None
     if any(
         kwargs[key]
         for key in [
@@ -690,14 +692,15 @@
     with ExitStack() as exit_stack:
         if override_system_timezone:
             exit_stack.enter_context(mock_system_timezone(override_system_timezone))
 
         server_termination_event = threading.Event()
         api_servicer = DagsterApiServer(
             server_termination_event=server_termination_event,
+            logger=logger,
             loadable_target_origin=loadable_target_origin,
             heartbeat=heartbeat,
             heartbeat_timeout=heartbeat_timeout,
             lazy_load_user_code=lazy_load_user_code,
             fixed_server_id=fixed_server_id,
             entry_point=(
                 get_python_environment_entry_point(sys.executable)
```

### Comparing `dagster-1.3.5/dagster/_cli/asset.py` & `dagster-1.3.6/dagster/_cli/asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_cli/config_scaffolder.py` & `dagster-1.3.6/dagster/_cli/config_scaffolder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_cli/debug.py` & `dagster-1.3.6/dagster/_cli/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_cli/dev.py` & `dagster-1.3.6/dagster/_cli/dev.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,18 @@
 
 @click.command(
     name="dev",
     help=(
         "Start a local deployment of Dagster, including dagit running on localhost and the"
         " dagster-daemon running in the background"
     ),
+    context_settings=dict(
+        max_content_width=120,
+        help_option_names=["--help"],  # Don't show '-h' since that's the dagit host
+    ),
 )
 @dev_command_options
 @click.option(
     "--code-server-log-level",
     help="Set the log level for code servers spun up by dagster services.",
     show_default=True,
     default="warning",
```

### Comparing `dagster-1.3.5/dagster/_cli/instance.py` & `dagster-1.3.6/dagster/_cli/instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_cli/job.py` & `dagster-1.3.6/dagster/_cli/job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_cli/load_handle.py` & `dagster-1.3.6/dagster/_cli/load_handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_cli/project.py` & `dagster-1.3.6/dagster/_cli/project.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_cli/run.py` & `dagster-1.3.6/dagster/_cli/run.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_cli/schedule.py` & `dagster-1.3.6/dagster/_cli/schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_cli/sensor.py` & `dagster-1.3.6/dagster/_cli/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_cli/utils.py` & `dagster-1.3.6/dagster/_cli/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_cli/workspace/cli_target.py` & `dagster-1.3.6/dagster/_cli/workspace/cli_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_config/__init__.py` & `dagster-1.3.6/dagster/_config/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_config/config_schema.py` & `dagster-1.3.6/dagster/_config/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_config/config_type.py` & `dagster-1.3.6/dagster/_config/config_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_config/errors.py` & `dagster-1.3.6/dagster/_config/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_config/evaluate_value_result.py` & `dagster-1.3.6/dagster/_config/evaluate_value_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_config/field.py` & `dagster-1.3.6/dagster/_config/field.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_config/field_utils.py` & `dagster-1.3.6/dagster/_config/field_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_config/post_process.py` & `dagster-1.3.6/dagster/_config/post_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_config/primitive_mapping.py` & `dagster-1.3.6/dagster/_config/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_config/pythonic_config/__init__.py` & `dagster-1.3.6/dagster/_config/pythonic_config/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_config/pythonic_config/attach_other_object_to_context.py` & `dagster-1.3.6/dagster/_config/pythonic_config/attach_other_object_to_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_config/pythonic_config/typing_utils.py` & `dagster-1.3.6/dagster/_config/pythonic_config/typing_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_config/pythonic_config/utils.py` & `dagster-1.3.6/dagster/_config/pythonic_config/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_config/snap.py` & `dagster-1.3.6/dagster/_config/snap.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_config/source.py` & `dagster-1.3.6/dagster/_config/source.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_config/stack.py` & `dagster-1.3.6/dagster/_config/stack.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_config/traversal_context.py` & `dagster-1.3.6/dagster/_config/traversal_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_config/type_printer.py` & `dagster-1.3.6/dagster/_config/type_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_config/validate.py` & `dagster-1.3.6/dagster/_config/validate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/assets.py` & `dagster-1.3.6/dagster/_core/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/code_pointer.py` & `dagster-1.3.6/dagster/_core/code_pointer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/container_context/config.py` & `dagster-1.3.6/dagster/_core/container_context/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/debug.py` & `dagster-1.3.6/dagster/_core/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/decorator_utils.py` & `dagster-1.3.6/dagster/_core/decorator_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/__init__.py` & `dagster-1.3.6/dagster/_core/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/asset_graph.py` & `dagster-1.3.6/dagster/_core/definitions/asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/asset_graph_subset.py` & `dagster-1.3.6/dagster/_core/definitions/asset_graph_subset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/asset_in.py` & `dagster-1.3.6/dagster/_core/definitions/asset_in.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/asset_layer.py` & `dagster-1.3.6/dagster/_core/definitions/asset_layer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/asset_out.py` & `dagster-1.3.6/dagster/_core/definitions/asset_out.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/asset_reconciliation_sensor.py` & `dagster-1.3.6/dagster/_core/definitions/asset_reconciliation_sensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     FreshnessAutoMaterializeCondition,
     MaxMaterializationsExceededAutoMaterializeCondition,
     MissingAutoMaterializeCondition,
     ParentMaterializedAutoMaterializeCondition,
     ParentOutdatedAutoMaterializeCondition,
 )
 from .decorators.sensor_decorator import sensor
-from .partition import PartitionsDefinition, PartitionsSubset
+from .partition import PartitionsDefinition, PartitionsSubset, SerializedPartitionsSubset
 from .run_request import RunRequest
 from .sensor_definition import DefaultSensorStatus, SensorDefinition
 from .utils import check_valid_name
 
 if TYPE_CHECKING:
     from dagster._core.instance import DagsterInstance, DynamicPartitionsStore
     from dagster._utils.caching_instance_queryer import CachingInstanceQueryer  # expensive import
@@ -61,36 +61,36 @@
 
 @whitelist_for_serdes
 class AutoMaterializeAssetEvaluation(NamedTuple):
     """Represents the results of the auto-materialize logic for a single asset.
 
     Properties:
         asset_key (AssetKey): The asset key that was evaluated.
-        conditions: The conditions that impact if the asset should be materialized, skipped, or
+        partition_subsets_by_condition: The conditions that impact if the asset should be materialized, skipped, or
             discarded. If the asset is partitioned, this will be a list of tuples, where the first
-            element is the condition and the second element is the set of partitions that the
-            condition applies to.
+            element is the condition and the second element is the serialized subset of partitions that the
+            condition applies to. If it's not partitioned, the second element will be None.
     """
 
     asset_key: AssetKey
-    conditions: Union[
-        Sequence[AutoMaterializeCondition],
-        Sequence[Tuple[AutoMaterializeCondition, PartitionsSubset]],
+    partition_subsets_by_condition: Sequence[
+        Tuple[AutoMaterializeCondition, Optional[SerializedPartitionsSubset]]
     ]
     num_requested: int
     num_skipped: int
     num_discarded: int
 
     @staticmethod
     def from_conditions(
         asset_graph: AssetGraph,
         asset_key: AssetKey,
         conditions_by_asset_partition: Mapping[
             AssetKeyPartitionKey, AbstractSet[AutoMaterializeCondition]
         ],
+        dynamic_partitions_store: "DynamicPartitionsStore",
     ) -> "AutoMaterializeAssetEvaluation":
         num_requested = 0
         num_skipped = 0
         num_discarded = 0
 
         for conditions in conditions_by_asset_partition.values():
             decision_types = {condition.decision_type for condition in conditions}
@@ -102,15 +102,18 @@
                 check.invariant(AutoMaterializeDecisionType.MATERIALIZE in decision_types)
                 num_requested += 1
 
         partitions_def = asset_graph.get_partitions_def(asset_key)
         if partitions_def is None:
             return AutoMaterializeAssetEvaluation(
                 asset_key=asset_key,
-                conditions=list(set().union(*conditions_by_asset_partition.values())),
+                partition_subsets_by_condition=[
+                    (condition, None)
+                    for condition in set().union(*conditions_by_asset_partition.values())
+                ],
                 num_requested=num_requested,
                 num_skipped=num_skipped,
                 num_discarded=num_discarded,
             )
         else:
             partition_keys_by_condition = defaultdict(set)
 
@@ -118,16 +121,25 @@
                 for condition in conditions:
                     partition_keys_by_condition[condition].add(
                         check.not_none(asset_partition.partition_key)
                     )
 
             return AutoMaterializeAssetEvaluation(
                 asset_key=asset_key,
-                conditions=[
-                    (condition, partitions_def.empty_subset().with_partition_keys(partition_keys))
+                partition_subsets_by_condition=[
+                    (
+                        condition,
+                        SerializedPartitionsSubset.from_subset(
+                            subset=partitions_def.empty_subset().with_partition_keys(
+                                partition_keys
+                            ),
+                            partitions_def=partitions_def,
+                            dynamic_partitions_store=dynamic_partitions_store,
+                        ),
+                    )
                     for condition, partition_keys in partition_keys_by_condition.items()
                 ],
                 num_requested=num_requested,
                 num_skipped=num_skipped,
                 num_discarded=num_discarded,
             )
 
@@ -219,14 +231,15 @@
         asset. Every value is the set of that asset's partitoins that have been requested by
         this sensor or have been materialized (even if not by this sensor).
     """
 
     latest_storage_id: Optional[int]
     materialized_or_requested_root_asset_keys: AbstractSet[AssetKey]
     materialized_or_requested_root_partitions_by_asset_key: Mapping[AssetKey, PartitionsSubset]
+    evaluation_id: Optional[int]
 
     def was_previously_materialized_or_requested(self, asset_key: AssetKey) -> bool:
         return asset_key in self.materialized_or_requested_root_asset_keys
 
     def get_never_requested_never_materialized_partitions(
         self,
         asset_key: AssetKey,
@@ -267,14 +280,15 @@
 
     def with_updates(
         self,
         latest_storage_id: Optional[int],
         run_requests: Sequence[RunRequest],
         newly_materialized_root_asset_keys: AbstractSet[AssetKey],
         newly_materialized_root_partitions_by_asset_key: Mapping[AssetKey, AbstractSet[str]],
+        evaluation_id: Optional[int],
         asset_graph: AssetGraph,
     ) -> "AssetReconciliationCursor":
         """Returns a cursor that represents this cursor plus the updates that have happened within the
         tick.
         """
         requested_root_partitions_by_asset_key: Dict[AssetKey, Set[str]] = defaultdict(set)
         requested_non_partitioned_root_assets: Set[AssetKey] = set()
@@ -324,31 +338,39 @@
                 "Latest storage ID should be >= previous latest storage ID",
             )
 
         return AssetReconciliationCursor(
             latest_storage_id=latest_storage_id or self.latest_storage_id,
             materialized_or_requested_root_asset_keys=result_materialized_or_requested_root_asset_keys,
             materialized_or_requested_root_partitions_by_asset_key=result_materialized_or_requested_root_partitions_by_asset_key,
+            evaluation_id=evaluation_id,
         )
 
     @classmethod
     def empty(cls) -> "AssetReconciliationCursor":
         return AssetReconciliationCursor(
             latest_storage_id=None,
             materialized_or_requested_root_partitions_by_asset_key={},
             materialized_or_requested_root_asset_keys=set(),
+            evaluation_id=0,
         )
 
     @classmethod
     def from_serialized(cls, cursor: str, asset_graph: AssetGraph) -> "AssetReconciliationCursor":
+        data = json.loads(cursor)
+        check.invariant(len(data) in [3, 4], "Invalid serialized cursor")
+
         (
             latest_storage_id,
             serialized_materialized_or_requested_root_asset_keys,
             serialized_materialized_or_requested_root_partitions_by_asset_key,
-        ) = json.loads(cursor)
+        ) = data[:3]
+
+        evaluation_id = data[3] if len(data) == 4 else None
+
         materialized_or_requested_root_partitions_by_asset_key = {}
         for (
             key_str,
             serialized_subset,
         ) in serialized_materialized_or_requested_root_partitions_by_asset_key.items():
             key = AssetKey.from_user_string(key_str)
             if key not in asset_graph.non_source_asset_keys:
@@ -371,26 +393,28 @@
         return cls(
             latest_storage_id=latest_storage_id,
             materialized_or_requested_root_asset_keys={
                 AssetKey.from_user_string(key_str)
                 for key_str in serialized_materialized_or_requested_root_asset_keys
             },
             materialized_or_requested_root_partitions_by_asset_key=materialized_or_requested_root_partitions_by_asset_key,
+            evaluation_id=evaluation_id,
         )
 
     def serialize(self) -> str:
         serializable_materialized_or_requested_root_partitions_by_asset_key = {
             key.to_user_string(): subset.serialize()
             for key, subset in self.materialized_or_requested_root_partitions_by_asset_key.items()
         }
         serialized = json.dumps(
             (
                 self.latest_storage_id,
                 [key.to_user_string() for key in self.materialized_or_requested_root_asset_keys],
                 serializable_materialized_or_requested_root_partitions_by_asset_key,
+                self.evaluation_id,
             )
         )
         return serialized
 
 
 def get_active_backfill_target_asset_graph_subset(
     instance: "DagsterInstance", asset_graph: AssetGraph
@@ -1087,16 +1111,19 @@
         run_requests,
         cursor.with_updates(
             latest_storage_id=latest_storage_id,
             run_requests=run_requests,
             asset_graph=asset_graph,
             newly_materialized_root_asset_keys=newly_materialized_root_asset_keys,
             newly_materialized_root_partitions_by_asset_key=newly_materialized_root_partitions_by_asset_key,
+            evaluation_id=cursor.evaluation_id + 1 if cursor.evaluation_id is not None else 0,
+        ),
+        build_auto_materialize_asset_evaluations(
+            asset_graph, conditions_by_asset_partition, dynamic_partitions_store=instance_queryer
         ),
-        build_auto_materialize_asset_evaluations(asset_graph, conditions_by_asset_partition),
     )
 
 
 def build_run_requests(
     asset_partitions: Iterable[AssetKeyPartitionKey],
     asset_graph: AssetGraph,
     run_tags: Optional[Mapping[str, str]],
@@ -1139,26 +1166,29 @@
 
 
 def build_auto_materialize_asset_evaluations(
     asset_graph: AssetGraph,
     conditions_by_asset_partition: Mapping[
         AssetKeyPartitionKey, AbstractSet[AutoMaterializeCondition]
     ],
+    dynamic_partitions_store: "DynamicPartitionsStore",
 ) -> Sequence[AutoMaterializeAssetEvaluation]:
     """Bundles up the conditions into AutoMaterializeAssetEvaluations."""
     conditions_by_asset_key: Dict[
         AssetKey, Dict[AssetKeyPartitionKey, AbstractSet[AutoMaterializeCondition]]
     ] = defaultdict(dict)
 
     # split into sub-dictionaries that hold only the conditions specific to each asset
     for asset_partition, conditions in conditions_by_asset_partition.items():
         conditions_by_asset_key[asset_partition.asset_key][asset_partition] = conditions
 
     return [
-        AutoMaterializeAssetEvaluation.from_conditions(asset_graph, asset_key, conditions)
+        AutoMaterializeAssetEvaluation.from_conditions(
+            asset_graph, asset_key, conditions, dynamic_partitions_store
+        )
         for asset_key, conditions in conditions_by_asset_key.items()
     ]
 
 
 @experimental
 def build_asset_reconciliation_sensor(
     asset_selection: AssetSelection,
```

### Comparing `dagster-1.3.5/dagster/_core/definitions/asset_selection.py` & `dagster-1.3.6/dagster/_core/definitions/asset_selection.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/asset_sensor_definition.py` & `dagster-1.3.6/dagster/_core/definitions/asset_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/assets.py` & `dagster-1.3.6/dagster/_core/definitions/assets.py`

 * *Files 2% similar despite different names*

```diff
@@ -922,43 +922,51 @@
             },
             freshness_policies_by_key=replaced_freshness_policies_by_key,
             auto_materialize_policies_by_key=replaced_auto_materialize_policies_by_key,
             descriptions_by_key=replaced_descriptions_by_key,
         )
 
     def _subset_op_backed_asset(
-        self, asset_subselection: AbstractSet[AssetKey]
+        self, asset_subselection: AbstractSet[AssetKey], selected_asset_keys: AbstractSet[AssetKey]
     ) -> "AssetsDefinition":
         """Creates a new AssetsDefinition which will only materialize the given asset keys. In some
         cases, this subset will have a new set of root assets, which were previously produced within
         the subset itself. In this case, we will create new inputs for those assets, and generate a
         new copy of the op with the new inputs.
+
+        Args:
+            asset_subselection (AbstractSet[AssetKey]): The set of asset keys that should be selected
+                from this AssetsDefinition.
+            selected_asset_keys (AbstractSet[AssetKey]): The total set of asset keys that have been
+                selected from the broader asset graph.
         """
         # the set of keys that are not selected but are upstream of the selected keys
         input_keys = {
             dep_key for key in asset_subselection for dep_key in self.asset_deps[key]
         }.difference(asset_subselection)
         ins = {}
 
         input_names_by_key = {v: k for k, v in self.keys_by_input_name.items()}
         output_names_by_key = {v: k for k, v in self.keys_by_output_name.items()}
         op_valid = True
         for input_key in input_keys:
             input_name = input_names_by_key.get(input_key)
-            if input_name is None:
-                # there is no input existing for this key, meaning this is something that is produced
-                # within the op if it is not subsetted. this requires us to create a new input, and
-                # therefore a new copy of the underlying op.
+            if input_name is not None:
+                # just copy over existing input
+                ins[input_name] = self.op.ins[input_name]
+            elif input_key in selected_asset_keys:
+                # There is no input existing for this key, meaning this is something that is produced
+                # within the op if it is not subsetted. If this input is part of the larger
+                # selection that we want to make a job out of, then this would require us to create
+                # a new input such that the dependency would be respected, and therefore a new copy
+                # of the underlying op.
                 op_valid = False
                 output_name = output_names_by_key[input_key]
                 ins[output_name] = In(Nothing)
                 input_names_by_key[input_key] = output_name
-            else:
-                # just copy over existing input
-                ins[input_name] = self.op.ins[input_name]
 
         # must create a new copy of the op
         if op_valid:
             op_def = self.op
         else:
             # create a hash of the selected keys to generate a unique name for this subsetted op
             suffix = hashlib.md5((str(list(sorted(asset_subselection)))).encode()).hexdigest()[-5:]
@@ -1078,15 +1086,15 @@
                 metadata_by_key=self.metadata_by_key,
                 freshness_policies_by_key=self.freshness_policies_by_key,
                 auto_materialize_policies_by_key=self.auto_materialize_policies_by_key,
                 descriptions_by_key=self.descriptions_by_key,
             )
         else:
             # multi_asset subsetting
-            return self._subset_op_backed_asset(asset_subselection)
+            return self._subset_op_backed_asset(asset_subselection, selected_asset_keys)
 
     @public
     def to_source_assets(self) -> Sequence[SourceAsset]:
         """Returns a SourceAsset for each asset in this definition.
 
         Each produced SourceAsset will have the same key, metadata, io_manager_key, etc. as the
         corresponding asset
```

### Comparing `dagster-1.3.5/dagster/_core/definitions/assets_job.py` & `dagster-1.3.6/dagster/_core/definitions/assets_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/auto_materialize_condition.py` & `dagster-1.3.6/dagster/_core/definitions/auto_materialize_condition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/auto_materialize_policy.py` & `dagster-1.3.6/dagster/_core/definitions/auto_materialize_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/cacheable_assets.py` & `dagster-1.3.6/dagster/_core/definitions/cacheable_assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/composition.py` & `dagster-1.3.6/dagster/_core/definitions/composition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/config.py` & `dagster-1.3.6/dagster/_core/definitions/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/configurable.py` & `dagster-1.3.6/dagster/_core/definitions/configurable.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/data_time.py` & `dagster-1.3.6/dagster/_core/definitions/data_time.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/data_version.py` & `dagster-1.3.6/dagster/_core/definitions/data_version.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/decorators/__init__.py` & `dagster-1.3.6/dagster/_core/definitions/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/decorators/asset_decorator.py` & `dagster-1.3.6/dagster/_core/definitions/decorators/asset_decorator.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from dagster._core.definitions.auto_materialize_policy import AutoMaterializePolicy
 from dagster._core.definitions.freshness_policy import FreshnessPolicy
 from dagster._core.definitions.metadata import ArbitraryMetadataMapping, MetadataUserInput
 from dagster._core.definitions.resource_annotation import (
     get_resource_args,
 )
 from dagster._core.errors import DagsterInvalidDefinitionError
-from dagster._core.storage.io_manager import IOManagerDefinition
 from dagster._core.types.dagster_type import DagsterType
 from dagster._utils.backcompat import (
     ExperimentalWarning,
     deprecation_warning,
     experimental_arg_warning,
 )
 
@@ -62,15 +61,15 @@
     ins: Optional[Mapping[str, AssetIn]] = ...,
     non_argument_deps: Optional[Union[Set[AssetKey], Set[str]]] = ...,
     metadata: Optional[Mapping[str, Any]] = ...,
     description: Optional[str] = ...,
     config_schema: Optional[UserConfigSchema] = None,
     required_resource_keys: Optional[Set[str]] = ...,
     resource_defs: Optional[Mapping[str, object]] = ...,
-    io_manager_def: Optional[IOManagerDefinition] = ...,
+    io_manager_def: Optional[object] = ...,
     io_manager_key: Optional[str] = ...,
     compute_kind: Optional[str] = ...,
     dagster_type: Optional[DagsterType] = ...,
     partitions_def: Optional[PartitionsDefinition] = ...,
     op_tags: Optional[Mapping[str, Any]] = ...,
     group_name: Optional[str] = ...,
     output_required: bool = ...,
@@ -90,15 +89,15 @@
     ins: Optional[Mapping[str, AssetIn]] = None,
     non_argument_deps: Optional[Union[Set[AssetKey], Set[str]]] = None,
     metadata: Optional[ArbitraryMetadataMapping] = None,
     description: Optional[str] = None,
     config_schema: Optional[UserConfigSchema] = None,
     required_resource_keys: Optional[Set[str]] = None,
     resource_defs: Optional[Mapping[str, object]] = None,
-    io_manager_def: Optional[IOManagerDefinition] = None,
+    io_manager_def: Optional[object] = None,
     io_manager_key: Optional[str] = None,
     compute_kind: Optional[str] = None,
     dagster_type: Optional[DagsterType] = None,
     partitions_def: Optional[PartitionsDefinition] = None,
     op_tags: Optional[Mapping[str, Any]] = None,
     group_name: Optional[str] = None,
     output_required: bool = True,
@@ -137,15 +136,15 @@
             op. If set, Dagster will check that config provided for the op matches this schema and fail
             if it does not. If not set, Dagster will accept any config provided for the op.
         metadata (Optional[Dict[str, Any]]): A dict of metadata entries for the asset.
         required_resource_keys (Optional[Set[str]]): Set of resource handles required by the op.
         io_manager_key (Optional[str]): The resource key of the IOManager used
             for storing the output of the op as an asset, and for loading it in downstream ops
             (default: "io_manager"). Only one of io_manager_key and io_manager_def can be provided.
-        io_manager_def (Optional[IOManagerDefinition]): (Experimental) The definition of the IOManager used for
+        io_manager_def (Optional[object]): (Experimental) The IOManager used for
             storing the output of the op as an asset,  and for loading it in
             downstream ops. Only one of io_manager_def and io_manager_key can be provided.
         compute_kind (Optional[str]): A string to represent the kind of computation that produces
             the asset, e.g. "dbt" or "spark". It will be displayed in Dagit as a badge on the asset.
         dagster_type (Optional[DagsterType]): Allows specifying type validation functions that
             will be executed on the output of the decorated function after it runs.
         partitions_def (Optional[PartitionsDefinition]): Defines the set of partition keys that
@@ -177,27 +176,26 @@
 
             @asset
             def my_asset(my_upstream_asset: int) -> int:
                 return my_upstream_asset + 1
     """
 
     def create_asset():
-        from dagster._core.execution.build_resources import wrap_resources_for_execution
-
         return _Asset(
             name=cast(Optional[str], name),  # (mypy bug that it can't infer name is Optional[str])
             key_prefix=key_prefix,
             ins=ins,
             non_argument_deps=_make_asset_keys(non_argument_deps),
             metadata=metadata,
             description=description,
             config_schema=config_schema,
             required_resource_keys=required_resource_keys,
-            resource_defs=wrap_resources_for_execution(resource_defs),
-            io_manager=io_manager_def or io_manager_key,
+            resource_defs=resource_defs,
+            io_manager_key=io_manager_key,
+            io_manager_def=io_manager_def,
             compute_kind=check.opt_str_param(compute_kind, "compute_kind"),
             dagster_type=dagster_type,
             partitions_def=partitions_def,
             op_tags=op_tags,
             group_name=group_name,
             output_required=output_required,
             freshness_policy=freshness_policy,
@@ -238,16 +236,17 @@
         key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
         ins: Optional[Mapping[str, AssetIn]] = None,
         non_argument_deps: Optional[Set[AssetKey]] = None,
         metadata: Optional[ArbitraryMetadataMapping] = None,
         description: Optional[str] = None,
         config_schema: Optional[UserConfigSchema] = None,
         required_resource_keys: Optional[Set[str]] = None,
-        resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
-        io_manager: Optional[Union[str, IOManagerDefinition]] = None,
+        resource_defs: Optional[Mapping[str, object]] = None,
+        io_manager_key: Optional[str] = None,
+        io_manager_def: Optional[object] = None,
         compute_kind: Optional[str] = None,
         dagster_type: Optional[DagsterType] = None,
         partitions_def: Optional[PartitionsDefinition] = None,
         op_tags: Optional[Mapping[str, Any]] = None,
         group_name: Optional[str] = None,
         output_required: bool = True,
         freshness_policy: Optional[FreshnessPolicy] = None,
@@ -263,64 +262,79 @@
         self.ins = ins or {}
         self.non_argument_deps = non_argument_deps
         self.metadata = metadata
         self.description = description
         self.required_resource_keys = check.opt_set_param(
             required_resource_keys, "required_resource_keys"
         )
-        self.io_manager = io_manager
+        self.io_manager_key = io_manager_key
+        self.io_manager_def = io_manager_def
         self.config_schema = config_schema
         self.compute_kind = compute_kind
         self.dagster_type = dagster_type
         self.partitions_def = partitions_def
         self.op_tags = op_tags
         self.resource_defs = dict(check.opt_mapping_param(resource_defs, "resource_defs"))
         self.group_name = group_name
         self.output_required = output_required
         self.freshness_policy = freshness_policy
         self.retry_policy = retry_policy
         self.auto_materialize_policy = auto_materialize_policy
         self.code_version = code_version
 
     def __call__(self, fn: Callable) -> AssetsDefinition:
-        from dagster._config.pythonic_config import validate_resource_annotated_function
+        from dagster._config.pythonic_config import (
+            validate_resource_annotated_function,
+        )
+        from dagster._core.execution.build_resources import wrap_resources_for_execution
 
         validate_resource_annotated_function(fn)
         asset_name = self.name or fn.__name__
 
         asset_ins = build_asset_ins(fn, self.ins or {}, self.non_argument_deps)
 
         out_asset_key = AssetKey(list(filter(None, [*(self.key_prefix or []), asset_name])))
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", category=ExperimentalWarning)
 
             arg_resource_keys = {arg.name for arg in get_resource_args(fn)}
 
             bare_required_resource_keys = set(self.required_resource_keys)
-            resource_defs_keys = set(self.resource_defs.keys())
+
+            resource_defs_dict = self.resource_defs
+            resource_defs_keys = set(resource_defs_dict.keys())
             decorator_resource_keys = bare_required_resource_keys | resource_defs_keys
 
+            io_manager_key = self.io_manager_key
+            if self.io_manager_def:
+                if not io_manager_key:
+                    io_manager_key = out_asset_key.to_python_identifier("io_manager")
+
+                if (
+                    io_manager_key in self.resource_defs
+                    and self.resource_defs[io_manager_key] != self.io_manager_def
+                ):
+                    raise DagsterInvalidDefinitionError(
+                        f"Provided conflicting definitions for io manager key '{io_manager_key}'."
+                        " Please provide only one definition per key."
+                    )
+
+                resource_defs_dict[io_manager_key] = self.io_manager_def
+
+            wrapped_resource_defs = wrap_resources_for_execution(resource_defs_dict)
+
             check.param_invariant(
                 len(bare_required_resource_keys) == 0 or len(arg_resource_keys) == 0,
                 (
                     "Cannot specify resource requirements in both @asset decorator and as arguments"
                     " to the decorated function"
                 ),
             )
 
-            if isinstance(self.io_manager, str):
-                io_manager_key = cast(str, self.io_manager)
-            elif self.io_manager is not None:
-                io_manager_def = check.inst_param(
-                    self.io_manager, "io_manager", IOManagerDefinition
-                )
-                io_manager_key = out_asset_key.to_python_identifier("io_manager")
-                self.resource_defs[io_manager_key] = cast(ResourceDefinition, io_manager_def)
-            else:
-                io_manager_key = DEFAULT_IO_MANAGER_KEY
+            io_manager_key = cast(str, io_manager_key) if io_manager_key else DEFAULT_IO_MANAGER_KEY
 
             out = Out(
                 metadata=self.metadata or {},
                 io_manager_key=io_manager_key,
                 dagster_type=self.dagster_type if self.dagster_type else NoValueSentinel,
                 description=self.description,
                 is_required=self.output_required,
@@ -357,15 +371,15 @@
 
         return AssetsDefinition.dagster_internal_init(
             keys_by_input_name=keys_by_input_name,
             keys_by_output_name={"result": out_asset_key},
             node_def=op,
             partitions_def=self.partitions_def,
             partition_mappings=partition_mappings if partition_mappings else None,
-            resource_defs=self.resource_defs,
+            resource_defs=wrapped_resource_defs,
             group_names_by_key={out_asset_key: self.group_name} if self.group_name else None,
             freshness_policies_by_key={out_asset_key: self.freshness_policy}
             if self.freshness_policy
             else None,
             auto_materialize_policies_by_key={out_asset_key: self.auto_materialize_policy}
             if self.auto_materialize_policy
             else None,
```

### Comparing `dagster-1.3.5/dagster/_core/definitions/decorators/config_mapping_decorator.py` & `dagster-1.3.6/dagster/_core/definitions/decorators/config_mapping_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/decorators/graph_decorator.py` & `dagster-1.3.6/dagster/_core/definitions/decorators/graph_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/decorators/hook_decorator.py` & `dagster-1.3.6/dagster/_core/definitions/decorators/hook_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/decorators/job_decorator.py` & `dagster-1.3.6/dagster/_core/definitions/decorators/job_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/decorators/op_decorator.py` & `dagster-1.3.6/dagster/_core/definitions/decorators/op_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/decorators/repository_decorator.py` & `dagster-1.3.6/dagster/_core/definitions/decorators/repository_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/decorators/schedule_decorator.py` & `dagster-1.3.6/dagster/_core/definitions/decorators/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/decorators/sensor_decorator.py` & `dagster-1.3.6/dagster/_core/definitions/decorators/sensor_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/decorators/source_asset_decorator.py` & `dagster-1.3.6/dagster/_core/definitions/decorators/source_asset_decorator.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,30 +5,29 @@
 from dagster._core.definitions.events import AssetKey, CoercibleToAssetKeyPrefix
 from dagster._core.definitions.metadata import (
     MetadataUserInput,
 )
 from dagster._core.definitions.resource_annotation import get_resource_args
 from dagster._core.definitions.resource_definition import ResourceDefinition
 from dagster._core.definitions.source_asset import SourceAsset, SourceAssetObserveFunction
-from dagster._core.storage.io_manager import IOManagerDefinition
 
 
 @overload
 def observable_source_asset(observe_fn: SourceAssetObserveFunction) -> SourceAsset:
     ...
 
 
 @overload
 def observable_source_asset(
     *,
     name: Optional[str] = ...,
     key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
     metadata: Optional[MetadataUserInput] = None,
     io_manager_key: Optional[str] = None,
-    io_manager_def: Optional[IOManagerDefinition] = None,
+    io_manager_def: Optional[object] = None,
     description: Optional[str] = None,
     group_name: Optional[str] = None,
     required_resource_keys: Optional[AbstractSet[str]] = None,
     resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
 ) -> "_ObservableSourceAsset":
     ...
 
@@ -37,15 +36,15 @@
 def observable_source_asset(
     observe_fn: Optional[SourceAssetObserveFunction] = None,
     *,
     name: Optional[str] = None,
     key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
     metadata: Optional[MetadataUserInput] = None,
     io_manager_key: Optional[str] = None,
-    io_manager_def: Optional[IOManagerDefinition] = None,
+    io_manager_def: Optional[object] = None,
     description: Optional[str] = None,
     group_name: Optional[str] = None,
     required_resource_keys: Optional[AbstractSet[str]] = None,
     resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
 ) -> Union[SourceAsset, "_ObservableSourceAsset"]:
     """Create a `SourceAsset` with an associated observation function.
 
@@ -95,15 +94,15 @@
 class _ObservableSourceAsset:
     def __init__(
         self,
         name: Optional[str] = None,
         key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
         metadata: Optional[MetadataUserInput] = None,
         io_manager_key: Optional[str] = None,
-        io_manager_def: Optional[IOManagerDefinition] = None,
+        io_manager_def: Optional[object] = None,
         description: Optional[str] = None,
         group_name: Optional[str] = None,
         required_resource_keys: Optional[AbstractSet[str]] = None,
         resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
     ):
         self.name = name
         if isinstance(key_prefix, str):
```

### Comparing `dagster-1.3.5/dagster/_core/definitions/definition_config_schema.py` & `dagster-1.3.6/dagster/_core/definitions/definition_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/definitions_class.py` & `dagster-1.3.6/dagster/_core/definitions/definitions_class.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/dependency.py` & `dagster-1.3.6/dagster/_core/definitions/dependency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/events.py` & `dagster-1.3.6/dagster/_core/definitions/events.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/executor_definition.py` & `dagster-1.3.6/dagster/_core/definitions/executor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/external_asset_graph.py` & `dagster-1.3.6/dagster/_core/definitions/external_asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/freshness_policy.py` & `dagster-1.3.6/dagster/_core/definitions/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/freshness_policy_sensor_definition.py` & `dagster-1.3.6/dagster/_core/definitions/freshness_policy_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/graph_definition.py` & `dagster-1.3.6/dagster/_core/definitions/graph_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/hook_definition.py` & `dagster-1.3.6/dagster/_core/definitions/hook_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/hook_invocation.py` & `dagster-1.3.6/dagster/_core/definitions/hook_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/inference.py` & `dagster-1.3.6/dagster/_core/definitions/inference.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/input.py` & `dagster-1.3.6/dagster/_core/definitions/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/instigation_logger.py` & `dagster-1.3.6/dagster/_core/definitions/instigation_logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/job_base.py` & `dagster-1.3.6/dagster/_core/definitions/job_base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/job_definition.py` & `dagster-1.3.6/dagster/_core/definitions/job_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,14 +205,15 @@
         }
         self._required_resource_keys = self._get_required_resource_keys(was_provided_resources)
 
         self._config_mapping = None
         self._partitioned_config = None
         self._run_config = None
         self._run_config_schema = None
+        self._original_config_argument = config
 
         if partitions_def:
             self._partitioned_config = PartitionedConfig.from_flexible_config(
                 config, partitions_def
             )
         else:
             if isinstance(config, ConfigMapping):
@@ -914,15 +915,15 @@
     def _copy(self, **kwargs: Any) -> "JobDefinition":
         # dict() calls copy dict props
         base_kwargs = dict(
             graph_def=self.graph,
             resource_defs=dict(self.resource_defs),
             executor_def=self._executor_def,
             logger_defs=self._loggers,
-            config=self._config_mapping or self._partitioned_config or self._run_config,
+            config=self._original_config_argument,
             name=self._name,
             description=self.description,
             tags=self.tags,
             metadata=self._metadata,
             hook_defs=self.hook_defs,
             op_retry_policy=self._op_retry_policy,
             version_strategy=self.version_strategy,
```

### Comparing `dagster-1.3.5/dagster/_core/definitions/load_assets_from_modules.py` & `dagster-1.3.6/dagster/_core/definitions/load_assets_from_modules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/logger_definition.py` & `dagster-1.3.6/dagster/_core/definitions/logger_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/logger_invocation.py` & `dagster-1.3.6/dagster/_core/definitions/logger_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/materialize.py` & `dagster-1.3.6/dagster/_core/definitions/materialize.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/metadata/__init__.py` & `dagster-1.3.6/dagster/_core/definitions/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/metadata/table.py` & `dagster-1.3.6/dagster/_core/definitions/metadata/table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/multi_asset_sensor_definition.py` & `dagster-1.3.6/dagster/_core/definitions/multi_asset_sensor_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,27 +287,27 @@
 
         # This method caches the initial unconsumed events for each asset key. To generate the
         # current unconsumed events, call get_trailing_unconsumed_events instead.
         if self._fetched_initial_unconsumed_events:
             return
 
         for asset_key in self._monitored_asset_keys:
-            event_records = self.instance.get_event_records(
-                EventRecordsFilter(
-                    event_type=DagsterEventType.ASSET_MATERIALIZATION,
-                    storage_ids=list(
-                        self._get_cursor(
-                            asset_key
-                        ).trailing_unconsumed_partitioned_event_ids.values()
-                    ),
-                )
-            )
-            self._initial_unconsumed_events_by_id.update(
-                {event_record.storage_id: event_record for event_record in event_records}
+            unconsumed_event_ids = list(
+                self._get_cursor(asset_key).trailing_unconsumed_partitioned_event_ids.values()
             )
+            if unconsumed_event_ids:
+                event_records = self.instance.get_event_records(
+                    EventRecordsFilter(
+                        event_type=DagsterEventType.ASSET_MATERIALIZATION,
+                        storage_ids=unconsumed_event_ids,
+                    )
+                )
+                self._initial_unconsumed_events_by_id.update(
+                    {event_record.storage_id: event_record for event_record in event_records}
+                )
 
         self._fetched_initial_unconsumed_events = True
 
     def _get_unconsumed_events_with_ids(
         self, event_ids: Sequence[int]
     ) -> Sequence["EventLogRecord"]:
         self._cache_initial_unconsumed_events()
@@ -365,14 +365,15 @@
         )
 
         if new_cursor is not None:
             # Cursor was not updated by this context object, so we do not need to update it
             self._cursor = new_cursor
             self._unpacked_cursor = MultiAssetSensorContextCursor(new_cursor, self)
             self._cursor_advance_state_mutation = MultiAssetSensorCursorAdvances()
+            self._fetched_initial_unconsumed_events = False
 
     @public
     def latest_materialization_records_by_key(
         self,
         asset_keys: Optional[Sequence[AssetKey]] = None,
     ) -> Mapping[AssetKey, Optional["EventLogRecord"]]:
         """Fetches the most recent materialization event record for each asset in asset_keys.
```

### Comparing `dagster-1.3.5/dagster/_core/definitions/multi_dimensional_partitions.py` & `dagster-1.3.6/dagster/_core/definitions/multi_dimensional_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/node_container.py` & `dagster-1.3.6/dagster/_core/definitions/node_container.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/node_definition.py` & `dagster-1.3.6/dagster/_core/definitions/node_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/observe.py` & `dagster-1.3.6/dagster/_core/definitions/observe.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/op_definition.py` & `dagster-1.3.6/dagster/_core/definitions/op_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/op_invocation.py` & `dagster-1.3.6/dagster/_core/definitions/op_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/op_selection.py` & `dagster-1.3.6/dagster/_core/definitions/op_selection.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/output.py` & `dagster-1.3.6/dagster/_core/definitions/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/partition.py` & `dagster-1.3.6/dagster/_core/definitions/partition.py`

 * *Files 1% similar despite different names*

```diff
@@ -894,14 +894,47 @@
 
     @classmethod
     @abstractmethod
     def empty_subset(cls, partitions_def: PartitionsDefinition[T_str]) -> "PartitionsSubset[T_str]":
         ...
 
 
+@whitelist_for_serdes
+class SerializedPartitionsSubset(NamedTuple):
+    serialized_subset: str
+    serialized_partitions_def_unique_id: str
+    serialized_partitions_def_class_name: str
+
+    @classmethod
+    def from_subset(
+        cls,
+        subset: PartitionsSubset,
+        partitions_def: PartitionsDefinition,
+        dynamic_partitions_store: DynamicPartitionsStore,
+    ):
+        return cls(
+            serialized_subset=subset.serialize(),
+            serialized_partitions_def_unique_id=partitions_def.get_serializable_unique_identifier(
+                dynamic_partitions_store
+            ),
+            serialized_partitions_def_class_name=partitions_def.__class__.__name__,
+        )
+
+    def can_deserialize(self, partitions_def: Optional[PartitionsDefinition]) -> bool:
+        if not partitions_def:
+            # Asset had a partitions definition at storage time, but no longer does
+            return False
+
+        return partitions_def.can_deserialize_subset(
+            self.serialized_subset,
+            serialized_partitions_def_unique_id=self.serialized_partitions_def_unique_id,
+            serialized_partitions_def_class_name=self.serialized_partitions_def_class_name,
+        )
+
+
 class DefaultPartitionsSubset(PartitionsSubset[T_str]):
     # Every time we change the serialization format, we should increment the version number.
     # This will ensure that we can gracefully degrade when deserializing old data.
     SERIALIZATION_VERSION = 1
 
     def __init__(
         self, partitions_def: PartitionsDefinition[T_str], subset: Optional[Set[T_str]] = None
```

### Comparing `dagster-1.3.5/dagster/_core/definitions/partition_mapping.py` & `dagster-1.3.6/dagster/_core/definitions/partition_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/partitioned_schedule.py` & `dagster-1.3.6/dagster/_core/definitions/partitioned_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/policy.py` & `dagster-1.3.6/dagster/_core/definitions/policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/reconstruct.py` & `dagster-1.3.6/dagster/_core/definitions/reconstruct.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/repository_definition/__init__.py` & `dagster-1.3.6/dagster/_core/definitions/repository_definition/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/repository_definition/caching_index.py` & `dagster-1.3.6/dagster/_core/definitions/repository_definition/caching_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/repository_definition/repository_data.py` & `dagster-1.3.6/dagster/_core/definitions/repository_definition/repository_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/repository_definition/repository_data_builder.py` & `dagster-1.3.6/dagster/_core/definitions/repository_definition/repository_data_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/repository_definition/repository_definition.py` & `dagster-1.3.6/dagster/_core/definitions/repository_definition/repository_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/repository_definition/valid_definitions.py` & `dagster-1.3.6/dagster/_core/definitions/repository_definition/valid_definitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/resolved_asset_deps.py` & `dagster-1.3.6/dagster/_core/definitions/resolved_asset_deps.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/resource_annotation.py` & `dagster-1.3.6/dagster/_core/definitions/resource_annotation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/resource_definition.py` & `dagster-1.3.6/dagster/_core/definitions/resource_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/resource_invocation.py` & `dagster-1.3.6/dagster/_core/definitions/resource_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/resource_requirement.py` & `dagster-1.3.6/dagster/_core/definitions/resource_requirement.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/run_config.py` & `dagster-1.3.6/dagster/_core/definitions/run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/run_config_schema.py` & `dagster-1.3.6/dagster/_core/definitions/run_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/run_request.py` & `dagster-1.3.6/dagster/_core/definitions/run_request.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/run_status_sensor_definition.py` & `dagster-1.3.6/dagster/_core/definitions/run_status_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/schedule_definition.py` & `dagster-1.3.6/dagster/_core/definitions/schedule_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import pendulum
 from typing_extensions import TypeAlias
 
 import dagster._check as check
 from dagster._annotations import deprecated, public
 from dagster._core.definitions.instigation_logger import InstigationLogger
 from dagster._core.definitions.resource_annotation import get_resource_args
-from dagster._core.definitions.scoped_resources_builder import Resources
+from dagster._core.definitions.scoped_resources_builder import Resources, ScopedResourcesBuilder
 from dagster._serdes import whitelist_for_serdes
 from dagster._utils import IHasInternalInit, ensure_gen
 from dagster._utils.backcompat import deprecation_warning
 from dagster._utils.merger import merge_dicts
 from dagster._utils.schedules import is_valid_cron_schedule
 
 from ..decorator_utils import has_at_least_one_parameter
@@ -238,17 +238,29 @@
         """
         from dagster._core.definitions.scoped_resources_builder import (
             IContainsGenerator,
         )
         from dagster._core.execution.build_resources import build_resources
 
         if not self._resources:
+            # Early exit if no resources are defined. This skips unnecessary initialization
+            # entirely. This allows users to run user code servers in cases where they
+            # do not have access to the instance if they use a subset of features do
+            # that do not require instance access. In this case, if they do not use
+            # resources on schedules they do not require the instance, so we do not
+            # instantiate it
+            #
+            # Tracking at https://github.com/dagster-io/dagster/issues/14345
+            if not self._resource_defs:
+                self._resources = ScopedResourcesBuilder.build_empty()
+                return self._resources
+
             instance = self.instance if self._instance or self._instance_ref else None
 
-            resources_cm = build_resources(resources=self._resource_defs or {}, instance=instance)
+            resources_cm = build_resources(resources=self._resource_defs, instance=instance)
             self._resources = self._exit_stack.enter_context(resources_cm)
 
             if isinstance(self._resources, IContainsGenerator) and not self._cm_scope_entered:
                 self._exit_stack.close()
                 raise DagsterInvariantViolationError(
                     "At least one provided resource is a generator, but attempting to access"
                     " resources outside of context manager scope. You can use the following syntax"
@@ -366,14 +378,15 @@
 
 
 def build_schedule_context(
     instance: Optional[DagsterInstance] = None,
     scheduled_execution_time: Optional[datetime] = None,
     resources: Optional[Mapping[str, object]] = None,
     repository_def: Optional["RepositoryDefinition"] = None,
+    instance_ref: Optional["InstanceRef"] = None,
 ) -> ScheduleEvaluationContext:
     """Builds schedule execution context using the provided parameters.
 
     The instance provided to ``build_schedule_context`` must be persistent;
     DagsterInstance.ephemeral() will result in an error.
 
     Args:
@@ -389,15 +402,19 @@
 
     """
     from dagster._core.execution.build_resources import wrap_resources_for_execution
 
     check.opt_inst_param(instance, "instance", DagsterInstance)
 
     return ScheduleEvaluationContext(
-        instance_ref=instance.get_ref() if instance and instance.is_persistent else None,
+        instance_ref=instance_ref
+        if instance_ref
+        else instance.get_ref()
+        if instance and instance.is_persistent
+        else None,
         scheduled_execution_time=check.opt_inst_param(
             scheduled_execution_time, "scheduled_execution_time", datetime
         ),
         resources=wrap_resources_for_execution(resources),
         repository_def=repository_def,
     )
```

### Comparing `dagster-1.3.5/dagster/_core/definitions/scoped_resources_builder.py` & `dagster-1.3.6/dagster/_core/definitions/scoped_resources_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/selector.py` & `dagster-1.3.6/dagster/_core/definitions/selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/sensor_definition.py` & `dagster-1.3.6/dagster/_core/definitions/sensor_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 )
 from dagster._core.definitions.resource_annotation import (
     get_resource_args,
 )
 from dagster._core.definitions.resource_definition import (
     Resources,
 )
+from dagster._core.definitions.scoped_resources_builder import ScopedResourcesBuilder
 from dagster._core.errors import (
     DagsterInvalidDefinitionError,
     DagsterInvalidInvocationError,
     DagsterInvalidSubsetError,
     DagsterInvariantViolationError,
 )
 from dagster._core.instance import DagsterInstance
@@ -239,14 +240,26 @@
 
             will work ok, but for a CM resource we must do
 
             with build_sensor_context(resources={"my_resource": my_cm_resource}) as context:
                 my_sensor(context)
             """
 
+            # Early exit if no resources are defined. This skips unnecessary initialization
+            # entirely. This allows users to run user code servers in cases where they
+            # do not have access to the instance if they use a subset of features do
+            # that do not require instance access. In this case, if they do not use
+            # resources on sensors they do not require the instance, so we do not
+            # instantiate it
+            #
+            # Tracking at https://github.com/dagster-io/dagster/issues/14345
+            if not self._resource_defs:
+                self._resources = ScopedResourcesBuilder.build_empty()
+                return self._resources
+
             instance = self.instance if self._instance or self._instance_ref else None
 
             resources_cm = build_resources(resources=self._resource_defs or {}, instance=instance)
             self._resources = self._exit_stack.enter_context(resources_cm)
 
             if isinstance(self._resources, IContainsGenerator) and not self._cm_scope_entered:
                 self._exit_stack.close()
@@ -987,14 +1000,15 @@
     instance: Optional[DagsterInstance] = None,
     cursor: Optional[str] = None,
     repository_name: Optional[str] = None,
     repository_def: Optional["RepositoryDefinition"] = None,
     sensor_name: Optional[str] = None,
     resources: Optional[Mapping[str, object]] = None,
     definitions: Optional["Definitions"] = None,
+    instance_ref: Optional["InstanceRef"] = None,
 ) -> SensorEvaluationContext:
     """Builds sensor execution context using the provided parameters.
 
     This function can be used to provide a context to the invocation of a sensor definition.If
     provided, the dagster instance must be persistent; DagsterInstance.ephemeral() will result in an
     error.
 
@@ -1029,15 +1043,15 @@
     repository_def = normalize_to_repository(
         check.opt_inst_param(definitions, "definitions", Definitions),
         check.opt_inst_param(repository_def, "repository_def", RepositoryDefinition),
         error_on_none=False,
     )
 
     return SensorEvaluationContext(
-        instance_ref=None,
+        instance_ref=instance_ref,
         last_completion_time=None,
         last_run_key=None,
         cursor=cursor,
         repository_name=repository_name,
         instance=instance,
         repository_def=repository_def,
         sensor_name=sensor_name,
```

### Comparing `dagster-1.3.5/dagster/_core/definitions/source_asset.py` & `dagster-1.3.6/dagster/_core/definitions/source_asset.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,29 +86,31 @@
     _node_def: Optional[OpDefinition]  # computed lazily
 
     def __init__(
         self,
         key: CoercibleToAssetKey,
         metadata: Optional[ArbitraryMetadataMapping] = None,
         io_manager_key: Optional[str] = None,
-        io_manager_def: Optional[IOManagerDefinition] = None,
+        io_manager_def: Optional[object] = None,
         description: Optional[str] = None,
         partitions_def: Optional[PartitionsDefinition] = None,
         group_name: Optional[str] = None,
         resource_defs: Optional[Mapping[str, object]] = None,
         observe_fn: Optional[SourceAssetObserveFunction] = None,
         # This is currently private because it is necessary for source asset observation functions,
         # but we have not yet decided on a final API for associated one or more ops with a source
         # asset. If we were to make this public, then we would have a canonical public
         # `required_resource_keys` used for observation that might end up conflicting with a set of
         # required resource keys for a different operation.
         _required_resource_keys: Optional[AbstractSet[str]] = None,
         # Add additional fields to with_resources and with_group below
     ):
-        from dagster._core.execution.build_resources import wrap_resources_for_execution
+        from dagster._core.execution.build_resources import (
+            wrap_resources_for_execution,
+        )
 
         if partitions_def is not None and observe_fn is not None:
             raise DagsterInvalidDefinitionError(
                 "Cannot specify a `partitions_def` for an observable source asset."
             )
 
         if resource_defs is not None:
@@ -117,34 +119,32 @@
         if io_manager_def is not None:
             experimental_arg_warning("io_manager_def", "SourceAsset.__new__")
 
         self.key = AssetKey.from_coercible(key)
         metadata = check.opt_mapping_param(metadata, "metadata", key_type=str)
         self.raw_metadata = metadata
         self.metadata = normalize_metadata(metadata, allow_invalid=True)
-        self.resource_defs = wrap_resources_for_execution(
-            dict(check.opt_mapping_param(resource_defs, "resource_defs"))
-        )
-        self._io_manager_def = check.opt_inst_param(
-            io_manager_def, "io_manager_def", IOManagerDefinition
-        )
-        if self._io_manager_def:
+
+        resource_defs_dict = dict(check.opt_mapping_param(resource_defs, "resource_defs"))
+        if io_manager_def:
             if not io_manager_key:
                 io_manager_key = self.key.to_python_identifier("io_manager")
 
             if (
-                io_manager_key in self.resource_defs
-                and self.resource_defs[io_manager_key] != io_manager_def
+                io_manager_key in resource_defs_dict
+                and resource_defs_dict[io_manager_key] != io_manager_def
             ):
                 raise DagsterInvalidDefinitionError(
                     f"Provided conflicting definitions for io manager key '{io_manager_key}'."
                     " Please provide only one definition per key."
                 )
 
-            self.resource_defs[io_manager_key] = self._io_manager_def
+            resource_defs_dict[io_manager_key] = io_manager_def
+
+        self.resource_defs = wrap_resources_for_execution(resource_defs_dict)
 
         self.io_manager_key = check.opt_str_param(io_manager_key, "io_manager_key")
         self.partitions_def = check.opt_inst_param(
             partitions_def, "partitions_def", PartitionsDefinition
         )
         self.group_name = validate_group_name(group_name)
         self.description = check.opt_str_param(description, "description")
```

### Comparing `dagster-1.3.5/dagster/_core/definitions/step_launcher.py` & `dagster-1.3.6/dagster/_core/definitions/step_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/target.py` & `dagster-1.3.6/dagster/_core/definitions/target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/time_window_partition_mapping.py` & `dagster-1.3.6/dagster/_core/definitions/time_window_partition_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/time_window_partitions.py` & `dagster-1.3.6/dagster/_core/definitions/time_window_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/unresolved_asset_job_definition.py` & `dagster-1.3.6/dagster/_core/definitions/unresolved_asset_job_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/utils.py` & `dagster-1.3.6/dagster/_core/definitions/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/definitions/version_strategy.py` & `dagster-1.3.6/dagster/_core/definitions/version_strategy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/errors.py` & `dagster-1.3.6/dagster/_core/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/event_api.py` & `dagster-1.3.6/dagster/_core/event_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,10 +135,10 @@
                 after_cursor, "after_cursor", (int, RunShardedEventsCursor)
             ),
             before_cursor=check.opt_inst_param(
                 before_cursor, "before_cursor", (int, RunShardedEventsCursor)
             ),
             after_timestamp=check.opt_float_param(after_timestamp, "after_timestamp"),
             before_timestamp=check.opt_float_param(before_timestamp, "before_timestamp"),
-            storage_ids=check.opt_sequence_param(storage_ids, "storage_ids", of_type=int),
+            storage_ids=check.opt_nullable_sequence_param(storage_ids, "storage_ids", of_type=int),
             tags=check.opt_mapping_param(tags, "tags", key_type=str),
         )
```

### Comparing `dagster-1.3.5/dagster/_core/events/__init__.py` & `dagster-1.3.6/dagster/_core/events/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/events/log.py` & `dagster-1.3.6/dagster/_core/events/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/events/utils.py` & `dagster-1.3.6/dagster/_core/events/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/api.py` & `dagster-1.3.6/dagster/_core/execution/api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/asset_backfill.py` & `dagster-1.3.6/dagster/_core/execution/asset_backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/backfill.py` & `dagster-1.3.6/dagster/_core/execution/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/build_resources.py` & `dagster-1.3.6/dagster/_core/execution/build_resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,16 +118,19 @@
     from dagster._config.pythonic_config import ConfigurableResourceFactory, PartialResource
 
     resources = check.opt_mapping_param(resources, "resources", key_type=str)
     resource_defs = {}
     # Wrap instantiated resource values in a resource definition.
     # If an instantiated IO manager is provided, wrap it in an IO manager definition.
     for resource_key, resource in resources.items():
+        # Wrap instantiated resource values in a resource definition.
+        # If an instantiated IO manager is provided, wrap it in an IO manager definition.
         if isinstance(resource, (ConfigurableResourceFactory, PartialResource)):
             resource_defs[resource_key] = resource.get_resource_definition()
         elif isinstance(resource, ResourceDefinition):
             resource_defs[resource_key] = resource
         elif isinstance(resource, IOManager):
             resource_defs[resource_key] = IOManagerDefinition.hardcoded_io_manager(resource)
         else:
             resource_defs[resource_key] = ResourceDefinition.hardcoded_resource(resource)
+
     return resource_defs
```

### Comparing `dagster-1.3.5/dagster/_core/execution/compute_logs.py` & `dagster-1.3.6/dagster/_core/execution/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/context/compute.py` & `dagster-1.3.6/dagster/_core/execution/context/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/context/hook.py` & `dagster-1.3.6/dagster/_core/execution/context/hook.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/context/init.py` & `dagster-1.3.6/dagster/_core/execution/context/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/context/input.py` & `dagster-1.3.6/dagster/_core/execution/context/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/context/invocation.py` & `dagster-1.3.6/dagster/_core/execution/context/invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/context/logger.py` & `dagster-1.3.6/dagster/_core/execution/context/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/context/output.py` & `dagster-1.3.6/dagster/_core/execution/context/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/context/system.py` & `dagster-1.3.6/dagster/_core/execution/context/system.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/context_creation_job.py` & `dagster-1.3.6/dagster/_core/execution/context_creation_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/execute_in_process.py` & `dagster-1.3.6/dagster/_core/execution/execute_in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/execute_in_process_result.py` & `dagster-1.3.6/dagster/_core/execution/execute_in_process_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/execution_result.py` & `dagster-1.3.6/dagster/_core/execution/execution_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/host_mode.py` & `dagster-1.3.6/dagster/_core/execution/host_mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/job_backfill.py` & `dagster-1.3.6/dagster/_core/execution/job_backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/job_execution_result.py` & `dagster-1.3.6/dagster/_core/execution/job_execution_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/memoization.py` & `dagster-1.3.6/dagster/_core/execution/memoization.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/plan/active.py` & `dagster-1.3.6/dagster/_core/execution/plan/active.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/plan/compute.py` & `dagster-1.3.6/dagster/_core/execution/plan/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/plan/compute_generator.py` & `dagster-1.3.6/dagster/_core/execution/plan/compute_generator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/plan/execute_plan.py` & `dagster-1.3.6/dagster/_core/execution/plan/execute_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/plan/execute_step.py` & `dagster-1.3.6/dagster/_core/execution/plan/execute_step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/plan/external_step.py` & `dagster-1.3.6/dagster/_core/execution/plan/external_step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/plan/handle.py` & `dagster-1.3.6/dagster/_core/execution/plan/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/plan/inputs.py` & `dagster-1.3.6/dagster/_core/execution/plan/inputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/plan/local_external_step_main.py` & `dagster-1.3.6/dagster/_core/execution/plan/local_external_step_main.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/plan/objects.py` & `dagster-1.3.6/dagster/_core/execution/plan/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/plan/outputs.py` & `dagster-1.3.6/dagster/_core/execution/plan/outputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/plan/plan.py` & `dagster-1.3.6/dagster/_core/execution/plan/plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/plan/state.py` & `dagster-1.3.6/dagster/_core/execution/plan/state.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/plan/step.py` & `dagster-1.3.6/dagster/_core/execution/plan/step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/plan/utils.py` & `dagster-1.3.6/dagster/_core/execution/plan/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/poll_compute_logs.py` & `dagster-1.3.6/dagster/_core/execution/poll_compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/resolve_versions.py` & `dagster-1.3.6/dagster/_core/execution/resolve_versions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/resources_init.py` & `dagster-1.3.6/dagster/_core/execution/resources_init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/retries.py` & `dagster-1.3.6/dagster/_core/execution/retries.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/run_cancellation_thread.py` & `dagster-1.3.6/dagster/_core/execution/run_cancellation_thread.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/stats.py` & `dagster-1.3.6/dagster/_core/execution/stats.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/tags.py` & `dagster-1.3.6/dagster/_core/execution/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/validate_run_config.py` & `dagster-1.3.6/dagster/_core/execution/validate_run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/watch_orphans.py` & `dagster-1.3.6/dagster/_core/execution/watch_orphans.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/execution/with_resources.py` & `dagster-1.3.6/dagster/_core/execution/with_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/executor/base.py` & `dagster-1.3.6/dagster/_core/executor/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/executor/child_process_executor.py` & `dagster-1.3.6/dagster/_core/executor/child_process_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/executor/in_process.py` & `dagster-1.3.6/dagster/_core/executor/in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/executor/init.py` & `dagster-1.3.6/dagster/_core/executor/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/executor/multiprocess.py` & `dagster-1.3.6/dagster/_core/executor/multiprocess.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/executor/step_delegating/step_delegating_executor.py` & `dagster-1.3.6/dagster/_core/executor/step_delegating/step_delegating_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/executor/step_delegating/step_handler/base.py` & `dagster-1.3.6/dagster/_core/executor/step_delegating/step_handler/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/host_representation/__init__.py` & `dagster-1.3.6/dagster/_core/host_representation/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/host_representation/code_location.py` & `dagster-1.3.6/dagster/_core/host_representation/code_location.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/host_representation/external.py` & `dagster-1.3.6/dagster/_core/host_representation/external.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/host_representation/external_data.py` & `dagster-1.3.6/dagster/_core/host_representation/external_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/host_representation/grpc_server_registry.py` & `dagster-1.3.6/dagster/_core/host_representation/grpc_server_registry.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,32 +2,33 @@
 
 import sys
 import threading
 import uuid
 from contextlib import AbstractContextManager
 from typing import (
     TYPE_CHECKING,
+    Any,
     Dict,
     List,
     NamedTuple,
     Optional,
     Union,
     cast,
 )
 
 import pendulum
 from typing_extensions import TypeGuard
 
 import dagster._check as check
-from dagster._core.errors import DagsterUserCodeProcessError
+from dagster._core.errors import DagsterUserCodeProcessError, DagsterUserCodeUnreachableError
 from dagster._core.host_representation.origin import (
     CodeLocationOrigin,
     ManagedGrpcPythonEnvCodeLocationOrigin,
 )
-from dagster._core.instance import DagsterInstance
+from dagster._core.instance import InstanceRef
 from dagster._core.types.loadable_target_origin import LoadableTargetOrigin
 from dagster._grpc.server import GrpcServerProcess
 from dagster._utils.error import SerializableErrorInfo, serializable_error_info_from_exc_info
 
 if TYPE_CHECKING:
     from dagster._grpc.client import DagsterGrpcClient
 
@@ -72,30 +73,34 @@
 
 
 # Creates local gRPC python processes from ManagedGrpcPythonEnvCodeLocationOrigins and shares
 # them between threads.
 class GrpcServerRegistry(AbstractContextManager):
     def __init__(
         self,
-        instance: DagsterInstance,
+        instance_ref: Optional[InstanceRef],
         # How long each process should run before a new process should be created the next
         # time a given origin is requested (which will pick up any changes that have been
         # made to the code)
         reload_interval: int,
         # How long the process can live without a heartbeat before it dies. You should ensure
         # that either heartbeat_ttl is greater than reload_interval (so that the process will reload
         # before it ends due to heartbeat failure), or if reload_interval is 0, that any processes
         # returned by this registry have at least one GrpcServerCodeLocation hitting the
         # server with a heartbeat while you want the process to stay running.
         heartbeat_ttl: int,
         # How long to wait for the server to start up and receive connections before timing out
         startup_timeout: int,
+        wait_for_processes_on_shutdown: bool,
         log_level: str = "INFO",
+        inject_env_vars_from_instance: bool = True,
+        container_image: Optional[str] = None,
+        container_context: Optional[Dict[str, Any]] = None,
     ):
-        self.instance = instance
+        self.instance_ref = instance_ref
 
         # map of servers being currently returned, keyed by origin ID
         self._active_entries: Dict[str, Union[ServerRegistryEntry, ErrorRegistryEntry]] = {}
 
         self._waited_for_processes = False
 
         check.invariant(
@@ -114,25 +119,29 @@
 
         self._all_processes: List[GrpcServerProcess] = []
 
         self._cleanup_thread_shutdown_event: Optional[threading.Event] = None
         self._cleanup_thread: Optional[threading.Thread] = None
 
         self._log_level = check.str_param(log_level, "log_level")
-
-        if self._reload_interval > 0:
-            self._cleanup_thread_shutdown_event = threading.Event()
-
-            self._cleanup_thread = threading.Thread(
-                target=self._clear_old_processes,
-                name="grpc-server-registry-cleanup",
-                args=(self._cleanup_thread_shutdown_event, self._reload_interval),
-            )
-            self._cleanup_thread.daemon = True
-            self._cleanup_thread.start()
+        self._inject_env_vars_from_instance = inject_env_vars_from_instance
+        self._container_image = container_image
+        self._container_context = container_context
+
+        self._wait_for_processes_on_shutdown = wait_for_processes_on_shutdown
+
+        self._cleanup_thread_shutdown_event = threading.Event()
+
+        self._cleanup_thread = threading.Thread(
+            target=self._clear_old_processes,
+            name="grpc-server-registry-cleanup",
+            args=(self._cleanup_thread_shutdown_event, self._reload_interval),
+        )
+        self._cleanup_thread.daemon = True
+        self._cleanup_thread.start()
 
     def supports_origin(
         self, code_location_origin: CodeLocationOrigin
     ) -> TypeGuard[ManagedGrpcPythonEnvCodeLocationOrigin]:
         return isinstance(code_location_origin, ManagedGrpcPythonEnvCodeLocationOrigin)
 
     @property
@@ -188,22 +197,25 @@
             refresh_server = loadable_target_origin != active_entry.loadable_target_origin
 
         new_server_id: Optional[str]
         if refresh_server:
             try:
                 new_server_id = str(uuid.uuid4())
                 server_process = GrpcServerProcess(
-                    instance_ref=self.instance.get_ref(),
+                    instance_ref=self.instance_ref,
                     location_name=code_location_origin.location_name,
                     loadable_target_origin=loadable_target_origin,
                     heartbeat=True,
                     heartbeat_timeout=self._heartbeat_ttl,
                     fixed_server_id=new_server_id,
                     startup_timeout=self._startup_timeout,
                     log_level=self._log_level,
+                    inject_env_vars_from_instance=self._inject_env_vars_from_instance,
+                    container_image=self._container_image,
+                    container_context=self._container_context,
                 )
                 self._all_processes.append(server_process)
                 self._active_entries[origin_id] = ServerRegistryEntry(
                     process=server_process,
                     loadable_target_origin=loadable_target_origin,
                     creation_timestamp=pendulum.now("UTC").timestamp(),
                     server_id=new_server_id,
@@ -241,15 +253,16 @@
 
             current_time = pendulum.now("UTC").timestamp()
             with self._lock:
                 origin_ids_to_clear: List[str] = []
 
                 for origin_id, entry in self._active_entries.items():
                     if (
-                        current_time - entry.creation_timestamp > reload_interval
+                        reload_interval > 0
+                        and current_time - entry.creation_timestamp > reload_interval
                     ):  # Use a different threshold for errors so they aren't cached as long?
                         origin_ids_to_clear.append(origin_id)
 
                 for origin_id in origin_ids_to_clear:
                     del self._active_entries[origin_id]
 
                 # Remove any dead processes from the all_processes map
@@ -264,19 +277,31 @@
                     del self._all_processes[index]
 
     def __exit__(self, exception_type, exception_value, traceback):
         if self._cleanup_thread:
             cast(threading.Event, self._cleanup_thread_shutdown_event).set()
             self._cleanup_thread.join()
 
+        self.shutdown_all_processes()
+
+        if self._wait_for_processes_on_shutdown:
+            self.wait_for_processes()
+
+    def shutdown_all_processes(self):
         for process in self._all_processes:
             process.shutdown_server()
 
-        if self.instance.code_server_settings.get("wait_for_local_processes_on_shutdown", False):
-            self.wait_for_processes()
+    def are_all_servers_shut_down(self) -> bool:
+        for process in self._all_processes:
+            try:
+                process.create_client().ping("")
+                return False
+            except DagsterUserCodeUnreachableError:
+                pass
+        return True
 
     def wait_for_processes(self) -> None:
         # Wait for any processes created by this registry. Generally not needed outside
         # of tests, since the processes have heartbeats and will end on their own once
         # they finish any outstanding executions.
         if self._waited_for_processes:
             return
```

### Comparing `dagster-1.3.5/dagster/_core/host_representation/grpc_server_state_subscriber.py` & `dagster-1.3.6/dagster/_core/host_representation/grpc_server_state_subscriber.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/host_representation/handle.py` & `dagster-1.3.6/dagster/_core/host_representation/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/host_representation/historical.py` & `dagster-1.3.6/dagster/_core/host_representation/historical.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/host_representation/job_index.py` & `dagster-1.3.6/dagster/_core/host_representation/job_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/host_representation/origin.py` & `dagster-1.3.6/dagster/_core/host_representation/origin.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
     NamedTuple,
     NoReturn,
     Optional,
     Sequence,
     cast,
 )
 
+import grpc
+
 import dagster._check as check
 from dagster._core.definitions.selector import PartitionSetSelector, RepositorySelector
 from dagster._core.errors import DagsterInvariantViolationError, DagsterUserCodeUnreachableError
 from dagster._core.instance.config import DEFAULT_LOCAL_CODE_SERVER_STARTUP_TIMEOUT
 from dagster._core.origin import DEFAULT_DAGSTER_ENTRY_POINT
 from dagster._core.types.loadable_target_origin import LoadableTargetOrigin
 from dagster._serdes import (
@@ -105,14 +107,18 @@
     def location_name(self) -> str:
         pass
 
     @abstractmethod
     def create_location(self) -> "CodeLocation":
         pass
 
+    @abstractmethod
+    def reload_location(self, instance: "DagsterInstance") -> "CodeLocation":
+        pass
+
 
 # Different storage name for backcompat
 @whitelist_for_serdes(storage_name="RegisteredRepositoryLocationOrigin")
 class RegisteredCodeLocationOrigin(
     NamedTuple("RegisteredCodeLocationOrigin", [("location_name", str)]),
     CodeLocationOrigin,
 ):
@@ -125,16 +131,22 @@
         return super(RegisteredCodeLocationOrigin, cls).__new__(cls, location_name)
 
     def get_display_metadata(self) -> Mapping[str, Any]:
         return {}
 
     def create_location(self) -> NoReturn:
         raise DagsterInvariantViolationError(
-            "A RegisteredCodeLocationOrigin does not have enough information to load its "
-            "repository location on its own."
+            "A RegisteredCodeLocationOrigin does not have enough information to create its "
+            "code location on its own."
+        )
+
+    def reload_location(self, instance: "DagsterInstance") -> NoReturn:
+        raise DagsterInvariantViolationError(
+            "A RegisteredCodeLocationOrigin does not have enough information to reload its "
+            "code location on its own."
         )
 
 
 # Different storage name for backcompat
 @whitelist_for_serdes(storage_name="InProcessRepositoryLocationOrigin")
 class InProcessCodeLocationOrigin(
     NamedTuple(
@@ -189,14 +201,17 @@
     def create_location(self) -> "InProcessCodeLocation":
         from dagster._core.host_representation.code_location import (
             InProcessCodeLocation,
         )
 
         return InProcessCodeLocation(self)
 
+    def reload_location(self, instance: "DagsterInstance") -> "InProcessCodeLocation":
+        raise NotImplementedError
+
 
 # Different storage name for backcompat
 @whitelist_for_serdes(storage_name="ManagedGrpcPythonEnvRepositoryLocationOrigin")
 class ManagedGrpcPythonEnvCodeLocationOrigin(
     NamedTuple(
         "_ManagedGrpcPythonEnvCodeLocationOrigin",
         [("loadable_target_origin", LoadableTargetOrigin), ("location_name", str)],
@@ -229,35 +244,44 @@
             "package_name": self.loadable_target_origin.package_name,
             "executable_path": self.loadable_target_origin.executable_path,
         }
         return {key: value for key, value in metadata.items() if value is not None}
 
     def create_location(self) -> NoReturn:
         raise DagsterInvariantViolationError(
-            "A ManagedGrpcPythonEnvCodeLocationOrigin needs a DynamicWorkspace"
-            " in order to create a handle."
+            "A ManagedGrpcPythonEnvCodeLocationOrigin needs a GrpcServerRegistry"
+            " in order to create a code location."
+        )
+
+    def reload_location(self, instance: "DagsterInstance") -> NoReturn:
+        raise DagsterInvariantViolationError(
+            "A ManagedGrpcPythonEnvCodeLocationOrigin needs a GrpcServerRegistry"
+            " in order to reload a code location."
         )
 
     @contextmanager
     def create_single_location(
         self,
         instance: "DagsterInstance",
     ) -> Iterator["GrpcServerCodeLocation"]:
         from dagster._core.workspace.context import DAGIT_GRPC_SERVER_HEARTBEAT_TTL
 
         from .code_location import GrpcServerCodeLocation
         from .grpc_server_registry import GrpcServerRegistry
 
         with GrpcServerRegistry(
-            instance=instance,
+            instance_ref=instance.get_ref(),
             reload_interval=0,
             heartbeat_ttl=DAGIT_GRPC_SERVER_HEARTBEAT_TTL,
-            startup_timeout=instance.code_server_process_startup_timeout
-            if instance
-            else DEFAULT_LOCAL_CODE_SERVER_STARTUP_TIMEOUT,
+            startup_timeout=(
+                instance.code_server_process_startup_timeout
+                if instance
+                else DEFAULT_LOCAL_CODE_SERVER_STARTUP_TIMEOUT
+            ),
+            wait_for_processes_on_shutdown=instance.wait_for_local_code_server_processes_on_shutdown,
         ) as grpc_server_registry:
             endpoint = grpc_server_registry.get_grpc_endpoint(self)
             with GrpcServerCodeLocation(
                 origin=self,
                 server_id=endpoint.server_id,
                 port=endpoint.port,
                 socket=endpoint.socket,
@@ -313,14 +337,33 @@
         metadata = {
             "host": self.host,
             "port": str(self.port) if self.port else None,
             "socket": self.socket,
         }
         return {key: value for key, value in metadata.items() if value is not None}
 
+    def reload_location(self, instance: "DagsterInstance") -> "GrpcServerCodeLocation":
+        from dagster._core.host_representation.code_location import (
+            GrpcServerCodeLocation,
+        )
+
+        try:
+            self.create_client().reload_code(timeout=instance.code_server_reload_timeout)
+        except Exception as e:
+            # Handle case when this is called against `dagster api grpc` servers that don't have this API method implemented
+            if (
+                isinstance(e.__cause__, grpc.RpcError)
+                and cast(grpc.RpcError, e.__cause__).code() == grpc.StatusCode.UNIMPLEMENTED
+            ):
+                pass
+            else:
+                raise
+
+        return GrpcServerCodeLocation(self)
+
     def create_location(self) -> "GrpcServerCodeLocation":
         from dagster._core.host_representation.code_location import (
             GrpcServerCodeLocation,
         )
 
         return GrpcServerCodeLocation(self)
```

### Comparing `dagster-1.3.5/dagster/_core/host_representation/represented.py` & `dagster-1.3.6/dagster/_core/host_representation/represented.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/instance/__init__.py` & `dagster-1.3.6/dagster/_core/instance/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -808,21 +808,28 @@
     @property
     def code_server_process_startup_timeout(self) -> int:
         return self.code_server_settings.get(
             "local_startup_timeout", DEFAULT_LOCAL_CODE_SERVER_STARTUP_TIMEOUT
         )
 
     @property
-    def run_monitoring_max_resume_run_attempts(self) -> int:
-        default_max_resume_run_attempts = 3 if self.run_launcher.supports_resume_run else 0
-        return self.run_monitoring_settings.get(
-            "max_resume_run_attempts", default_max_resume_run_attempts
+    def code_server_reload_timeout(self) -> int:
+        return self.code_server_settings.get(
+            "reload_timeout", DEFAULT_LOCAL_CODE_SERVER_STARTUP_TIMEOUT
         )
 
     @property
+    def wait_for_local_code_server_processes_on_shutdown(self) -> bool:
+        return self.code_server_settings.get("wait_for_local_processes_on_shutdown", False)
+
+    @property
+    def run_monitoring_max_resume_run_attempts(self) -> int:
+        return self.run_monitoring_settings.get("max_resume_run_attempts", 0)
+
+    @property
     def run_monitoring_poll_interval_seconds(self) -> int:
         return self.run_monitoring_settings.get("poll_interval_seconds", 120)
 
     @property
     def cancellation_thread_poll_interval_seconds(self) -> int:
         return self.get_settings("run_monitoring").get(
             "cancellation_thread_poll_interval_seconds", 10
```

### Comparing `dagster-1.3.5/dagster/_core/instance/config.py` & `dagster-1.3.6/dagster/_core/instance/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -246,25 +246,55 @@
         return default_retention_settings
 
 
 def sensors_daemon_config() -> Field:
     return Field(
         {
             "use_threads": Field(Bool, is_required=False, default_value=False),
-            "num_workers": Field(int, is_required=False),
+            "num_workers": Field(
+                int,
+                is_required=False,
+                description=(
+                    "How many threads to use to process ticks from multiple sensors in parallel"
+                ),
+            ),
+            "num_submit_workers": Field(
+                int,
+                is_required=False,
+                description=(
+                    "How many threads to use to submit runs from sensor ticks. Can be used to"
+                    " decrease latency when a sensor emits multiple run requests within a single"
+                    " tick."
+                ),
+            ),
         },
         is_required=False,
     )
 
 
 def schedules_daemon_config() -> Field:
     return Field(
         {
             "use_threads": Field(Bool, is_required=False, default_value=False),
-            "num_workers": Field(int, is_required=False),
+            "num_workers": Field(
+                int,
+                is_required=False,
+                description=(
+                    "How many threads to use to process ticks from multiple schedules in parallel"
+                ),
+            ),
+            "num_submit_workers": Field(
+                int,
+                is_required=False,
+                description=(
+                    "How many threads to use to submit runs from schedule ticks. Can be used to"
+                    " decrease latency when a schedule emits multiple run requests within a single"
+                    " tick."
+                ),
+            ),
         },
         is_required=False,
     )
 
 
 def secrets_loader_config_schema() -> Field:
     return Field(
```

### Comparing `dagster-1.3.5/dagster/_core/instance/ref.py` & `dagster-1.3.6/dagster/_core/instance/ref.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/instance_for_test.py` & `dagster-1.3.6/dagster/_core/instance_for_test.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/launcher/base.py` & `dagster-1.3.6/dagster/_core/launcher/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/launcher/default_run_launcher.py` & `dagster-1.3.6/dagster/_core/launcher/default_run_launcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 from typing_extensions import Self
 
 import dagster._seven as seven
 from dagster import (
     _check as check,
 )
 from dagster._config.config_schema import UserConfigSchema
-from dagster._core.errors import DagsterInvariantViolationError, DagsterLaunchFailedError
+from dagster._core.errors import (
+    DagsterInvariantViolationError,
+    DagsterLaunchFailedError,
+    DagsterUserCodeProcessError,
+)
 from dagster._core.storage.dagster_run import DagsterRun
 from dagster._core.storage.tags import GRPC_INFO_TAG
 from dagster._serdes import (
     ConfigurableClass,
     deserialize_value,
 )
 from dagster._serdes.config_class import ConfigurableClassData
@@ -174,14 +178,18 @@
                 cls=self.__class__,
             )
             return False
 
         res = deserialize_value(
             client.cancel_execution(CancelExecutionRequest(run_id=run_id)), CancelExecutionResult
         )
+
+        if res.serializable_error_info:
+            raise DagsterUserCodeProcessError.from_error_info(res.serializable_error_info)
+
         return res.success
 
     def join(self, timeout=30):
         # If this hasn't been initialized at all, we can just do a noop
         if not self.has_instance:
             return
```

### Comparing `dagster-1.3.5/dagster/_core/launcher/sync_in_memory_run_launcher.py` & `dagster-1.3.6/dagster/_core/launcher/sync_in_memory_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/log_manager.py` & `dagster-1.3.6/dagster/_core/log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/nux.py` & `dagster-1.3.6/dagster/_core/nux.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/origin.py` & `dagster-1.3.6/dagster/_core/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/run_coordinator/base.py` & `dagster-1.3.6/dagster/_core/run_coordinator/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/run_coordinator/default_run_coordinator.py` & `dagster-1.3.6/dagster/_core/run_coordinator/default_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/run_coordinator/queued_run_coordinator.py` & `dagster-1.3.6/dagster/_core/run_coordinator/queued_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/scheduler/__init__.py` & `dagster-1.3.6/dagster/_core/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/scheduler/execution.py` & `dagster-1.3.6/dagster/_core/scheduler/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/scheduler/instigation.py` & `dagster-1.3.6/dagster/_core/scheduler/instigation.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,18 @@
     InstigatorType as InstigatorType,
     SkipReason as SkipReason,
 )
 from dagster._core.definitions.selector import InstigatorSelector, RepositorySelector
 from dagster._core.host_representation.origin import ExternalInstigatorOrigin
 from dagster._serdes import create_snapshot_id
 from dagster._serdes.serdes import (
+    deserialize_value,
     whitelist_for_serdes,
 )
-from dagster._utils import xor
+from dagster._utils import datetime_as_float, xor
 from dagster._utils.error import SerializableErrorInfo
 from dagster._utils.merger import merge_dicts
 
 InstigatorData: TypeAlias = Union["ScheduleInstigatorData", "SensorInstigatorData"]
 
 
 @whitelist_for_serdes(old_storage_names={"JobStatus"})
@@ -588,9 +589,22 @@
         check.invariant(
             status == TickStatus.SKIPPED,
             "Tick status was not SKIPPED but skip_reason was provided",
         )
 
 
 class AutoMaterializeAssetEvaluationRecord(NamedTuple):
+    id: int
     evaluation: AutoMaterializeAssetEvaluation
     evaluation_id: int
+    timestamp: float
+
+    @classmethod
+    def from_db_row(cls, row):
+        return cls(
+            id=row["id"],
+            evaluation=deserialize_value(
+                row["asset_evaluation_body"], AutoMaterializeAssetEvaluation
+            ),
+            evaluation_id=row["evaluation_id"],
+            timestamp=datetime_as_float(row["create_timestamp"]),
+        )
```

### Comparing `dagster-1.3.5/dagster/_core/scheduler/scheduler.py` & `dagster-1.3.6/dagster/_core/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/secrets/env_file.py` & `dagster-1.3.6/dagster/_core/secrets/env_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/selector/subset_selector.py` & `dagster-1.3.6/dagster/_core/selector/subset_selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/snap/__init__.py` & `dagster-1.3.6/dagster/_core/snap/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/snap/dagster_types.py` & `dagster-1.3.6/dagster/_core/snap/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/snap/dep_snapshot.py` & `dagster-1.3.6/dagster/_core/snap/dep_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/snap/execution_plan_snapshot.py` & `dagster-1.3.6/dagster/_core/snap/execution_plan_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/snap/job_snapshot.py` & `dagster-1.3.6/dagster/_core/snap/job_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/snap/mode.py` & `dagster-1.3.6/dagster/_core/snap/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/snap/node.py` & `dagster-1.3.6/dagster/_core/snap/node.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/snap/snap_to_yaml.py` & `dagster-1.3.6/dagster/_core/snap/snap_to_yaml.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/DEVELOPING.md` & `dagster-1.3.6/dagster/_core/storage/DEVELOPING.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/README.md` & `dagster-1.3.6/dagster/_core/storage/alembic/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/env.py` & `dagster-1.3.6/dagster/_core/storage/alembic/env.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/001_initial_1.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/001_initial_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/031_add_kvs_table.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/031_add_kvs_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py` & `dagster-1.3.6/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/asset_value_loader.py` & `dagster-1.3.6/dagster/_core/storage/asset_value_loader.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/base_storage.py` & `dagster-1.3.6/dagster/_core/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/branching/branching_io_manager.py` & `dagster-1.3.6/dagster/_core/storage/branching/branching_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/captured_log_manager.py` & `dagster-1.3.6/dagster/_core/storage/captured_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/cloud_storage_compute_log_manager.py` & `dagster-1.3.6/dagster/_core/storage/cloud_storage_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/compute_log_manager.py` & `dagster-1.3.6/dagster/_core/storage/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/config.py` & `dagster-1.3.6/dagster/_core/storage/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/dagster_run.py` & `dagster-1.3.6/dagster/_core/storage/dagster_run.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/db_io_manager.py` & `dagster-1.3.6/dagster/_core/storage/db_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/event_log/__init__.py` & `dagster-1.3.6/dagster/_core/storage/event_log/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/event_log/base.py` & `dagster-1.3.6/dagster/_core/storage/event_log/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/event_log/in_memory.py` & `dagster-1.3.6/dagster/_core/storage/event_log/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/event_log/migration.py` & `dagster-1.3.6/dagster/_core/storage/event_log/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/event_log/polling_event_watcher.py` & `dagster-1.3.6/dagster/_core/storage/event_log/polling_event_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/event_log/schema.py` & `dagster-1.3.6/dagster/_core/storage/event_log/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/event_log/sql_event_log.py` & `dagster-1.3.6/dagster/_core/storage/event_log/sql_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini` & `dagster-1.3.6/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py` & `dagster-1.3.6/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py` & `dagster-1.3.6/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/file_manager.py` & `dagster-1.3.6/dagster/_core/storage/file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/fs_io_manager.py` & `dagster-1.3.6/dagster/_core/storage/fs_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/input_manager.py` & `dagster-1.3.6/dagster/_core/storage/input_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/io_manager.py` & `dagster-1.3.6/dagster/_core/storage/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/legacy_storage.py` & `dagster-1.3.6/dagster/_core/storage/legacy_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/local_compute_log_manager.py` & `dagster-1.3.6/dagster/_core/storage/local_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/mem_io_manager.py` & `dagster-1.3.6/dagster/_core/storage/mem_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/memoizable_io_manager.py` & `dagster-1.3.6/dagster/_core/storage/memoizable_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/migration/utils.py` & `dagster-1.3.6/dagster/_core/storage/migration/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/noop_compute_log_manager.py` & `dagster-1.3.6/dagster/_core/storage/noop_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/output_manager.py` & `dagster-1.3.6/dagster/_core/storage/output_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/partition_status_cache.py` & `dagster-1.3.6/dagster/_core/storage/partition_status_cache.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/root.py` & `dagster-1.3.6/dagster/_core/storage/root.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/root_input_manager.py` & `dagster-1.3.6/dagster/_core/storage/root_input_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/runs/base.py` & `dagster-1.3.6/dagster/_core/storage/runs/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/runs/in_memory.py` & `dagster-1.3.6/dagster/_core/storage/runs/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/runs/migration.py` & `dagster-1.3.6/dagster/_core/storage/runs/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/runs/schema.py` & `dagster-1.3.6/dagster/_core/storage/runs/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/runs/sql_run_storage.py` & `dagster-1.3.6/dagster/_core/storage/runs/sql_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/runs/sqlite/alembic/alembic.ini` & `dagster-1.3.6/dagster/_core/storage/runs/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py` & `dagster-1.3.6/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/schedules/base.py` & `dagster-1.3.6/dagster/_core/storage/schedules/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -133,14 +133,18 @@
         Args:
             origin_id (str): The id of the instigator target to delete
             selector_id (str): The logical instigator identifier
             before (datetime): All ticks before this datetime will get purged
             tick_statuses (Optional[List[TickStatus]]): The tick statuses to wipe
         """
 
+    @property
+    def supports_auto_materialize_asset_evaluations(self) -> bool:
+        return True
+
     @abc.abstractmethod
     def add_auto_materialize_asset_evaluations(
         self,
         evaluation_id: int,
         asset_evaluations: Sequence[AutoMaterializeAssetEvaluation],
     ) -> None:
         """Add asset policy evaluations to storage."""
```

### Comparing `dagster-1.3.5/dagster/_core/storage/schedules/migration.py` & `dagster-1.3.6/dagster/_core/storage/schedules/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/schedules/schema.py` & `dagster-1.3.6/dagster/_core/storage/schedules/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     db.Column("type", db.String(63)),
     db.Column("timestamp", db.types.TIMESTAMP),
     db.Column("tick_body", db.Text),
     db.Column("create_timestamp", db.DateTime, server_default=get_current_timestamp()),
     db.Column("update_timestamp", db.DateTime, server_default=get_current_timestamp()),
 )
 
-AssetPolicyEvaluationsTable = db.Table(
+AssetDaemonAssetEvaluationsTable = db.Table(
     "asset_daemon_asset_evaluations",
     ScheduleStorageSqlMetadata,
     db.Column(
         "id",
         db.BigInteger().with_variant(sqlite.INTEGER(), "sqlite"),
         primary_key=True,
         autoincrement=True,
@@ -85,11 +85,11 @@
     mysql_length=32,
 )
 db.Index("idx_job_tick_timestamp", JobTickTable.c.job_origin_id, JobTickTable.c.timestamp)
 db.Index("idx_tick_selector_timestamp", JobTickTable.c.selector_id, JobTickTable.c.timestamp)
 
 db.Index(
     "idx_asset_daemon_asset_evaluations_asset_key_evaluation_id",
-    AssetPolicyEvaluationsTable.c.asset_key,
-    AssetPolicyEvaluationsTable.c.evaluation_id,
+    AssetDaemonAssetEvaluationsTable.c.asset_key,
+    AssetDaemonAssetEvaluationsTable.c.evaluation_id,
     unique=True,
 )
```

### Comparing `dagster-1.3.5/dagster/_core/storage/schedules/sql_schedule_storage.py` & `dagster-1.3.6/dagster/_core/storage/schedules/sql_schedule_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 from .migration import (
     OPTIONAL_SCHEDULE_DATA_MIGRATIONS,
     REQUIRED_SCHEDULE_DATA_MIGRATIONS,
     SCHEDULE_JOBS_SELECTOR_ID,
     SCHEDULE_TICKS_SELECTOR_ID,
 )
 from .schema import (
-    AssetPolicyEvaluationsTable,
+    AssetDaemonAssetEvaluationsTable,
     InstigatorsTable,
     JobTable,
     JobTickTable,
     SecondaryIndexMigrationTable,
 )
 
 T_NamedTuple = TypeVar("T_NamedTuple", bound=NamedTuple)
@@ -281,14 +281,18 @@
         with self.connect() as conn:
             return self._has_instigators_table(conn)
 
     def _has_instigators_table(self, conn: Connection) -> bool:
         table_names = db.inspect(conn).get_table_names()
         return "instigators" in table_names
 
+    def _has_asset_daemon_asset_evaluations_table(self, conn: Connection) -> bool:
+        table_names = db.inspect(conn).get_table_names()
+        return "asset_daemon_asset_evaluations" in table_names
+
     def get_batch_ticks(
         self,
         selector_ids: Sequence[str],
         limit: Optional[int] = None,
         statuses: Optional[Sequence[TickStatus]] = None,
     ) -> Mapping[str, Sequence[InstigatorTick]]:
         check.sequence_param(selector_ids, "selector_ids", of_type=str)
@@ -451,24 +455,29 @@
             )
         else:
             query = query.where(JobTickTable.c.job_origin_id == origin_id)
 
         with self.connect() as conn:
             conn.execute(query)
 
+    @property
+    def supports_auto_materialize_asset_evaluations(self) -> bool:
+        with self.connect() as conn:
+            return self._has_asset_daemon_asset_evaluations_table(conn)
+
     def add_auto_materialize_asset_evaluations(
         self,
         evaluation_id: int,
         asset_evaluations: Sequence[AutoMaterializeAssetEvaluation],
     ):
         if not asset_evaluations:
             return
 
         with self.connect() as conn:
-            bulk_insert = AssetPolicyEvaluationsTable.insert().values(
+            bulk_insert = AssetDaemonAssetEvaluationsTable.insert().values(
                 [
                     {
                         "evaluation_id": evaluation_id,
                         "asset_key": evaluation.asset_key.to_string(),
                         "asset_evaluation_body": serialize_value(evaluation),
                         "num_requested": evaluation.num_requested,
                         "num_skipped": evaluation.num_skipped,
@@ -482,44 +491,40 @@
     def get_auto_materialize_asset_evaluations(
         self, asset_key: AssetKey, limit: int, cursor: Optional[int] = None
     ) -> Sequence[AutoMaterializeAssetEvaluationRecord]:
         with self.connect() as conn:
             query = (
                 db.select(
                     [
-                        AssetPolicyEvaluationsTable.c.asset_evaluation_body,
-                        AssetPolicyEvaluationsTable.c.evaluation_id,
+                        AssetDaemonAssetEvaluationsTable.c.id,
+                        AssetDaemonAssetEvaluationsTable.c.asset_evaluation_body,
+                        AssetDaemonAssetEvaluationsTable.c.evaluation_id,
+                        AssetDaemonAssetEvaluationsTable.c.create_timestamp,
                     ]
                 )
-                .where(AssetPolicyEvaluationsTable.c.asset_key == asset_key.to_string())
-                .order_by(AssetPolicyEvaluationsTable.c.evaluation_id.desc())
+                .where(AssetDaemonAssetEvaluationsTable.c.asset_key == asset_key.to_string())
+                .order_by(AssetDaemonAssetEvaluationsTable.c.evaluation_id.desc())
             ).limit(limit)
 
             if cursor:
-                query = query.where(AssetPolicyEvaluationsTable.c.evaluation_id < cursor)
+                query = query.where(AssetDaemonAssetEvaluationsTable.c.evaluation_id < cursor)
 
             rows = conn.execute(query)
-            return [
-                AutoMaterializeAssetEvaluationRecord(
-                    evaluation=deserialize_value(
-                        row["asset_evaluation_body"], AutoMaterializeAssetEvaluation
-                    ),
-                    evaluation_id=row["evaluation_id"],
-                )
-                for row in rows
-            ]
+            return [AutoMaterializeAssetEvaluationRecord.from_db_row(row) for row in rows]
 
     def wipe(self) -> None:
         """Clears the schedule storage."""
         with self.connect() as conn:
             # https://stackoverflow.com/a/54386260/324449
             conn.execute(JobTable.delete())
             conn.execute(JobTickTable.delete())
             if self._has_instigators_table(conn):
                 conn.execute(InstigatorsTable.delete())
+            if self._has_asset_daemon_asset_evaluations_table(conn):
+                conn.execute(AssetDaemonAssetEvaluationsTable.delete())
 
     # MIGRATIONS
 
     def has_secondary_index_table(self) -> bool:
         with self.connect() as conn:
             return "secondary_indexes" in db.inspect(conn).get_table_names()
```

### Comparing `dagster-1.3.5/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini` & `dagster-1.3.6/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py` & `dagster-1.3.6/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/sql.py` & `dagster-1.3.6/dagster/_core/storage/sql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/sqlite.py` & `dagster-1.3.6/dagster/_core/storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/sqlite_storage.py` & `dagster-1.3.6/dagster/_core/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/tags.py` & `dagster-1.3.6/dagster/_core/storage/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/temp_file_manager.py` & `dagster-1.3.6/dagster/_core/storage/temp_file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/storage/upath_io_manager.py` & `dagster-1.3.6/dagster/_core/storage/upath_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/system_config/composite_descent.py` & `dagster-1.3.6/dagster/_core/system_config/composite_descent.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/system_config/objects.py` & `dagster-1.3.6/dagster/_core/system_config/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/telemetry.py` & `dagster-1.3.6/dagster/_core/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/telemetry_upload.py` & `dagster-1.3.6/dagster/_core/telemetry_upload.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/test_utils.py` & `dagster-1.3.6/dagster/_core/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -298,14 +298,28 @@
 
 def today_at_midnight(timezone_name="UTC") -> "DateTime":
     check.str_param(timezone_name, "timezone_name")
     now = pendulum.now(timezone_name)
     return create_pendulum_time(now.year, now.month, now.day, tz=now.timezone.name)
 
 
+from dagster._core.storage.runs import SqliteRunStorage
+
+
+class ExplodeOnInitRunStorage(SqliteRunStorage):
+    def __init__(self, inst_data: Optional[ConfigurableClassData] = None):
+        raise NotImplementedError("Init was called")
+
+    @classmethod
+    def from_config_value(
+        cls, inst_data: Optional[ConfigurableClassData], config_value
+    ) -> "SqliteRunStorage":
+        raise NotImplementedError("from_config_value was called")
+
+
 class ExplodingRunLauncher(RunLauncher, ConfigurableClass):
     def __init__(self, inst_data: Optional[ConfigurableClassData] = None):
         self._inst_data = inst_data
 
         super().__init__()
 
     @property
```

### Comparing `dagster-1.3.5/dagster/_core/types/builtin_config_schemas.py` & `dagster-1.3.6/dagster/_core/types/builtin_config_schemas.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/types/config_schema.py` & `dagster-1.3.6/dagster/_core/types/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/types/dagster_type.py` & `dagster-1.3.6/dagster/_core/types/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/types/decorator.py` & `dagster-1.3.6/dagster/_core/types/decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/types/loadable_target_origin.py` & `dagster-1.3.6/dagster/_core/types/loadable_target_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/types/primitive_mapping.py` & `dagster-1.3.6/dagster/_core/types/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/types/python_dict.py` & `dagster-1.3.6/dagster/_core/types/python_dict.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/types/python_set.py` & `dagster-1.3.6/dagster/_core/types/python_set.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/types/python_tuple.py` & `dagster-1.3.6/dagster/_core/types/python_tuple.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/types/transform_typing.py` & `dagster-1.3.6/dagster/_core/types/transform_typing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/utility_ops.py` & `dagster-1.3.6/dagster/_core/utility_ops.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/utils.py` & `dagster-1.3.6/dagster/_core/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/workspace/autodiscovery.py` & `dagster-1.3.6/dagster/_core/workspace/autodiscovery.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/workspace/config_schema.py` & `dagster-1.3.6/dagster/_core/workspace/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/workspace/context.py` & `dagster-1.3.6/dagster/_core/workspace/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import sys
 import threading
 import time
 import warnings
 from abc import ABC, abstractmethod
 from contextlib import ExitStack
 from itertools import count
@@ -29,15 +30,18 @@
     GrpcServerRegistry,
 )
 from dagster._core.host_representation.grpc_server_state_subscriber import (
     LocationStateChangeEvent,
     LocationStateChangeEventType,
     LocationStateSubscriber,
 )
-from dagster._core.host_representation.origin import GrpcServerCodeLocationOrigin
+from dagster._core.host_representation.origin import (
+    GrpcServerCodeLocationOrigin,
+    ManagedGrpcPythonEnvCodeLocationOrigin,
+)
 from dagster._core.instance import DagsterInstance
 from dagster._utils.error import SerializableErrorInfo, serializable_error_info_from_exc_info
 
 from .load_target import WorkspaceLoadTarget
 from .permissions import (
     PermissionResult,
     get_location_scoped_user_permissions,
@@ -189,16 +193,16 @@
         return entry.origin.is_reload_supported if entry else False
 
     def is_shutdown_supported(self, name: str) -> bool:
         entry = self.get_location_entry(name)
         return entry.origin.is_shutdown_supported if entry else False
 
     def reload_code_location(self, name: str) -> "BaseWorkspaceRequestContext":
-        # This method reloads the location on the process context, and returns a new
-        # request context created from the updated process context
+        # This method signals to the remote gRPC server that it should reload its
+        # code, and returns a new request context created from the updated process context
         self.process_context.reload_code_location(name)
         return self.process_context.create_request_context()
 
     def shutdown_code_location(self, name: str):
         self.process_context.shutdown_code_location(name)
 
     def reload_workspace(self) -> Self:
@@ -449,43 +453,45 @@
             workspace_load_target, "workspace_load_target", WorkspaceLoadTarget
         )
 
         self._read_only = read_only
 
         self._version = version
 
-        # Guards changes to _location_dict, _location_error_dict, and _location_origin_dict
+        # Guards changes to _location_entry_dict, _watch_thread_shutdown_events and _watch_threads
         self._lock = threading.Lock()
-
-        # Only ever set up by main thread
         self._watch_thread_shutdown_events: Dict[str, threading.Event] = {}
         self._watch_threads: Dict[str, threading.Thread] = {}
 
         self._state_subscriber_id_iter = count()
         self._state_subscribers: Dict[int, LocationStateSubscriber] = {}
         self.add_state_subscriber(LocationStateSubscriber(self._location_state_events_handler))
 
         if grpc_server_registry:
             self._grpc_server_registry: GrpcServerRegistry = check.inst_param(
                 grpc_server_registry, "grpc_server_registry", GrpcServerRegistry
             )
         else:
             self._grpc_server_registry = self._stack.enter_context(
                 GrpcServerRegistry(
-                    instance=self._instance,
+                    instance_ref=self._instance.get_ref(),
                     reload_interval=0,
                     heartbeat_ttl=DAGIT_GRPC_SERVER_HEARTBEAT_TTL,
                     startup_timeout=instance.code_server_process_startup_timeout,
                     log_level=code_server_log_level,
+                    wait_for_processes_on_shutdown=instance.wait_for_local_code_server_processes_on_shutdown,
                 )
             )
 
         self._location_entry_dict: Dict[str, CodeLocationEntry] = {}
         self._update_workspace(
-            {origin.location_name: self._load_location(origin) for origin in self._origins}
+            {
+                origin.location_name: self._load_location(origin, reload=False)
+                for origin in self._origins
+            }
         )
 
     @property
     def workspace_load_target(self) -> Optional[WorkspaceLoadTarget]:
         return self._workspace_load_target
 
     @property
@@ -497,35 +503,14 @@
         self._state_subscribers[token] = subscriber
         return token
 
     def rm_state_subscriber(self, token: int) -> None:
         if token in self._state_subscribers:
             del self._state_subscribers[token]
 
-    def _create_location_from_origin(self, origin: CodeLocationOrigin) -> Optional[CodeLocation]:
-        if not self._grpc_server_registry.supports_origin(origin):
-            return origin.create_location()
-        else:
-            endpoint = (
-                self._grpc_server_registry.reload_grpc_endpoint(origin)
-                if self._grpc_server_registry.supports_reload
-                else self._grpc_server_registry.get_grpc_endpoint(origin)
-            )
-
-            return GrpcServerCodeLocation(
-                origin=origin,
-                server_id=endpoint.server_id,
-                port=endpoint.port,
-                socket=endpoint.socket,
-                host=endpoint.host,
-                heartbeat=True,
-                watch_server=False,
-                grpc_server_registry=self._grpc_server_registry,
-            )
-
     @property
     def instance(self) -> DagsterInstance:
         return self._instance
 
     @property
     def read_only(self) -> bool:
         return self._read_only
@@ -574,20 +559,40 @@
                 )
             ),
         )
         self._watch_thread_shutdown_events[location_name] = shutdown_event
         self._watch_threads[location_name] = watch_thread
         watch_thread.start()
 
-    def _load_location(self, origin: CodeLocationOrigin) -> CodeLocationEntry:
+    def _load_location(self, origin: CodeLocationOrigin, reload: bool) -> CodeLocationEntry:
         location_name = origin.location_name
         location = None
         error = None
         try:
-            location = self._create_location_from_origin(origin)
+            if isinstance(origin, ManagedGrpcPythonEnvCodeLocationOrigin):
+                endpoint = (
+                    self._grpc_server_registry.reload_grpc_endpoint(origin)
+                    if reload
+                    else self._grpc_server_registry.get_grpc_endpoint(origin)
+                )
+                location = GrpcServerCodeLocation(
+                    origin=origin,
+                    server_id=endpoint.server_id,
+                    port=endpoint.port,
+                    socket=endpoint.socket,
+                    host=endpoint.host,
+                    heartbeat=True,
+                    watch_server=False,
+                    grpc_server_registry=self._grpc_server_registry,
+                )
+            else:
+                location = (
+                    origin.reload_location(self.instance) if reload else origin.create_location()
+                )
+
         except Exception:
             error = serializable_error_info_from_exc_info(sys.exc_info())
             warnings.warn(
                 "Error loading repository location {location_name}:{error_string}".format(
                     location_name=location_name, error_string=error.to_string()
                 )
             )
@@ -631,28 +636,28 @@
         with self._lock:
             return (
                 location_name in self._location_entry_dict
                 and self._location_entry_dict[location_name].load_error is not None
             )
 
     def reload_code_location(self, name: str) -> None:
-        # Can be called from a background thread
-        new = self._load_location(self._location_entry_dict[name].origin)
+        new = self._load_location(self._location_entry_dict[name].origin, reload=True)
         with self._lock:
             # Relying on GC to clean up the old location once nothing else
             # is referencing it
             self._location_entry_dict[name] = new
 
     def shutdown_code_location(self, name: str) -> None:
         with self._lock:
             self._location_entry_dict[name].origin.shutdown_server()
 
     def reload_workspace(self) -> None:
         updated_locations = {
-            origin.location_name: self._load_location(origin) for origin in self._origins
+            origin.location_name: self._load_location(origin, reload=True)
+            for origin in self._origins
         }
         self._update_workspace(updated_locations)
 
     def _update_workspace(self, new_locations: Dict[str, CodeLocationEntry]):
         # minimize lock time by only holding while swapping data old to new
         with self._lock:
             previous_events = self._watch_thread_shutdown_events
@@ -697,15 +702,27 @@
             LocationStateChangeEventType.LOCATION_UPDATED,
             LocationStateChangeEventType.LOCATION_ERROR,
         ):
             # In case of an updated location, reload the handle to get updated repository data and
             # re-attach a subscriber
             # In case of a location error, just reload the handle in order to update the workspace
             # with the correct error messages
-            self.reload_code_location(event.location_name)
+            logging.getLogger("dagit").info(
+                f"Received {event.event_type} event for location {event.location_name}, refreshing"
+            )
+            self.refresh_code_location(event.location_name)
+
+    def refresh_code_location(self, name: str) -> None:
+        # This method reloads Dagit's copy of the code from the remote gRPC server without
+        # restarting it, and returns a new request context created from the updated process context
+        new = self._load_location(self._location_entry_dict[name].origin, reload=False)
+        with self._lock:
+            # Relying on GC to clean up the old location once nothing else
+            # is referencing it
+            self._location_entry_dict[name] = new
 
     def __enter__(self):
         return self
 
     def __exit__(self, exception_type, exception_value, traceback):
         self._update_workspace({})  # update to empty to close all current locations
         self._stack.close()
```

### Comparing `dagster-1.3.5/dagster/_core/workspace/load.py` & `dagster-1.3.6/dagster/_core/workspace/load.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/workspace/load_target.py` & `dagster-1.3.6/dagster/_core/workspace/load_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/workspace/permissions.py` & `dagster-1.3.6/dagster/_core/workspace/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_core/workspace/workspace.py` & `dagster-1.3.6/dagster/_core/workspace/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_daemon/__init__.py` & `dagster-1.3.6/dagster/_daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_daemon/asset_daemon.py` & `dagster-1.3.6/dagster/_daemon/asset_daemon.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         raw_cursor = persisted_info.get(CURSOR_KEY)
         cursor = (
             AssetReconciliationCursor.from_serialized(raw_cursor, asset_graph)
             if raw_cursor
             else AssetReconciliationCursor.empty()
         )
 
-        run_requests, new_cursor, _ = reconcile(
+        run_requests, new_cursor, evaluations = reconcile(
             asset_graph=asset_graph,
             target_asset_keys=target_asset_keys,
             instance=instance,
             cursor=cursor,
             run_tags=None,
         )
```

### Comparing `dagster-1.3.5/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py` & `dagster-1.3.6/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_daemon/auto_run_reexecution/event_log_consumer.py` & `dagster-1.3.6/dagster/_daemon/auto_run_reexecution/event_log_consumer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_daemon/backfill.py` & `dagster-1.3.6/dagster/_daemon/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_daemon/cli/__init__.py` & `dagster-1.3.6/dagster/_daemon/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_daemon/controller.py` & `dagster-1.3.6/dagster/_daemon/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,19 +63,20 @@
     ]
 
 
 def create_daemon_grpc_server_registry(
     instance: DagsterInstance, code_server_log_level: str = "INFO"
 ) -> GrpcServerRegistry:
     return GrpcServerRegistry(
-        instance=instance,
+        instance_ref=instance.get_ref(),
         reload_interval=DAEMON_GRPC_SERVER_RELOAD_INTERVAL,
         heartbeat_ttl=DAEMON_GRPC_SERVER_HEARTBEAT_TTL,
         startup_timeout=instance.code_server_process_startup_timeout,
         log_level=code_server_log_level,
+        wait_for_processes_on_shutdown=instance.wait_for_local_code_server_processes_on_shutdown,
     )
 
 
 @contextmanager
 def daemon_controller_from_instance(
     instance: DagsterInstance,
     workspace_load_target: WorkspaceLoadTarget,
```

### Comparing `dagster-1.3.5/dagster/_daemon/daemon.py` & `dagster-1.3.6/dagster/_daemon/daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_daemon/monitoring/monitoring_daemon.py` & `dagster-1.3.6/dagster/_daemon/monitoring/monitoring_daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py` & `dagster-1.3.6/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_daemon/sensor.py` & `dagster-1.3.6/dagster/_daemon/sensor.py`

 * *Files 4% similar despite different names*

```diff
@@ -251,25 +251,33 @@
     """Helper function that performs sensor evaluations on a tighter loop, while reusing grpc locations
     within a given daemon interval.  Rather than relying on the daemon machinery to run the
     iteration loop every 30 seconds, sensors are continuously evaluated, every 5 seconds. We rely on
     each sensor definition's min_interval to check that sensor evaluations are spaced appropriately.
     """
     sensor_state_lock = threading.Lock()
     sensor_tick_futures: Dict[str, Future] = {}
+    submit_threadpool_executor = None
+    threadpool_executor = None
     with ExitStack() as stack:
         settings = workspace_process_context.instance.get_settings("sensors")
         if settings.get("use_threads"):
             threadpool_executor = stack.enter_context(
                 ThreadPoolExecutor(
                     max_workers=settings.get("num_workers"),
                     thread_name_prefix="sensor_daemon_worker",
                 )
             )
-        else:
-            threadpool_executor = None
+            num_submit_workers = settings.get("num_submit_workers")
+            if num_submit_workers:
+                submit_threadpool_executor = stack.enter_context(
+                    ThreadPoolExecutor(
+                        max_workers=settings.get("num_submit_workers"),
+                        thread_name_prefix="sensor_submit_worker",
+                    )
+                )
 
         last_verbose_time = None
         while True:
             start_time = pendulum.now("UTC").timestamp()
             if until and start_time >= until:
                 # provide a way of organically ending the loop to support test environment
                 break
@@ -278,14 +286,15 @@
             verbose_logs_iteration = (
                 last_verbose_time is None or start_time - last_verbose_time > VERBOSE_LOGS_INTERVAL
             )
             yield from execute_sensor_iteration(
                 workspace_process_context,
                 logger,
                 threadpool_executor=threadpool_executor,
+                submit_threadpool_executor=submit_threadpool_executor,
                 sensor_tick_futures=sensor_tick_futures,
                 sensor_state_lock=sensor_state_lock,
                 log_verbose_checks=verbose_logs_iteration,
             )
             # Yield to check for heartbeats in case there were no yields within
             # execute_sensor_iteration
             yield None
@@ -302,14 +311,15 @@
             yield None
 
 
 def execute_sensor_iteration(
     workspace_process_context: IWorkspaceProcessContext,
     logger: logging.Logger,
     threadpool_executor: Optional[ThreadPoolExecutor] = None,
+    submit_threadpool_executor: Optional[ThreadPoolExecutor] = None,
     sensor_tick_futures: Optional[Dict[str, Future]] = None,
     sensor_state_lock: Optional[threading.Lock] = None,
     log_verbose_checks: bool = True,
     debug_crash_flags: Optional[DebugCrashFlags] = None,
 ):
     instance = workspace_process_context.instance
 
@@ -426,14 +436,15 @@
                 workspace_process_context,
                 logger,
                 external_sensor,
                 sensor_state,
                 sensor_state_lock,
                 sensor_debug_crash_flags,
                 tick_retention_settings,
+                submit_threadpool_executor,
             )
             sensor_tick_futures[external_sensor.selector_id] = future
             yield
 
         else:
             # evaluate the sensors in a loop, synchronously, yielding to allow the sensor daemon to
             # heartbeat
@@ -441,49 +452,53 @@
                 workspace_process_context,
                 logger,
                 external_sensor,
                 sensor_state,
                 sensor_state_lock,
                 sensor_debug_crash_flags,
                 tick_retention_settings,
+                submit_threadpool_executor=None,
             )
 
 
 def _process_tick(
     workspace_process_context: IWorkspaceProcessContext,
     logger: logging.Logger,
     external_sensor: ExternalSensor,
     sensor_state: InstigatorState,
     sensor_state_lock: threading.Lock,
     sensor_debug_crash_flags: Optional[SingleInstigatorDebugCrashFlags],
     tick_retention_settings,
+    submit_threadpool_executor: Optional[ThreadPoolExecutor],
 ):
     # evaluate the tick immediately, but from within a thread.  The main thread should be able to
     # heartbeat to keep the daemon alive
-    list(
+    return list(
         _process_tick_generator(
             workspace_process_context,
             logger,
             external_sensor,
             sensor_state,
             sensor_state_lock,
             sensor_debug_crash_flags,
             tick_retention_settings,
+            submit_threadpool_executor,
         )
     )
 
 
 def _process_tick_generator(
     workspace_process_context: IWorkspaceProcessContext,
     logger: logging.Logger,
     external_sensor: ExternalSensor,
     sensor_state: InstigatorState,
     sensor_state_lock: threading.Lock,
     sensor_debug_crash_flags: Optional[SingleInstigatorDebugCrashFlags],
     tick_retention_settings,
+    submit_threadpool_executor: Optional[ThreadPoolExecutor],
 ):
     instance = workspace_process_context.instance
     error_info = None
     with sensor_state_lock:
         # acquire the lock to avoid a race condition where we're updating the recently touched
         # timestamp on the sensor state, but clobbering it with an older timestamp which might open
         # us up to a new evaluation being delegated within the minimum interval
@@ -518,14 +533,15 @@
         ) as tick_context:
             _check_for_debug_crash(sensor_debug_crash_flags, "TICK_HELD")
             yield from _evaluate_sensor(
                 workspace_process_context,
                 tick_context,
                 external_sensor,
                 sensor_state,
+                submit_threadpool_executor,
                 sensor_debug_crash_flags,
             )
 
     except Exception:
         error_info = serializable_error_info_from_exc_info(sys.exc_info())
         logger.exception(f"Sensor daemon caught an error for sensor {external_sensor.name}")
 
@@ -558,19 +574,85 @@
                 cursor=instigator_data.cursor if instigator_data else None,
                 last_tick_start_timestamp=now.timestamp(),
             )
         )
     )
 
 
+class SubmitRunRequestResult(NamedTuple):
+    run_key: Optional[str]
+    error_info: Optional[SerializableErrorInfo]
+    run: Union[SkippedSensorRun, DagsterRun]
+
+
+def _submit_run_request(
+    run_request: RunRequest,
+    workspace_process_context: IWorkspaceProcessContext,
+    external_sensor: ExternalSensor,
+    code_location: CodeLocation,
+    existing_runs_by_key,
+    logger,
+    sensor_debug_crash_flags,
+) -> SubmitRunRequestResult:
+    instance = workspace_process_context.instance
+    sensor_origin = external_sensor.get_external_origin()
+
+    target_data: ExternalTargetData = check.not_none(
+        external_sensor.get_target_data(run_request.job_name)
+    )
+
+    job_subset_selector = JobSubsetSelector(
+        location_name=code_location.name,
+        repository_name=sensor_origin.external_repository_origin.repository_name,
+        job_name=target_data.job_name,
+        op_selection=target_data.op_selection,
+        asset_selection=run_request.asset_selection,
+    )
+    external_job = code_location.get_external_job(job_subset_selector)
+    run = _get_or_create_sensor_run(
+        logger,
+        instance,
+        code_location,
+        external_sensor,
+        external_job,
+        run_request,
+        target_data,
+        existing_runs_by_key,
+    )
+
+    if isinstance(run, SkippedSensorRun):
+        return SubmitRunRequestResult(run_key=run_request.run_key, error_info=None, run=run)
+
+    _check_for_debug_crash(sensor_debug_crash_flags, "RUN_CREATED")
+
+    error_info = None
+    try:
+        logger.info(f"Launching run for {external_sensor.name}")
+        instance.submit_run(run.run_id, workspace_process_context.create_request_context())
+        logger.info(
+            "Completed launch of run {run_id} for {sensor_name}".format(
+                run_id=run.run_id, sensor_name=external_sensor.name
+            )
+        )
+    except Exception:
+        error_info = serializable_error_info_from_exc_info(sys.exc_info())
+        logger.error(
+            f"Run {run.run_id} created successfully but failed to launch: {str(error_info)}"
+        )
+
+    _check_for_debug_crash(sensor_debug_crash_flags, "RUN_LAUNCHED")
+    return SubmitRunRequestResult(run_key=run_request.run_key, error_info=error_info, run=run)
+
+
 def _evaluate_sensor(
     workspace_process_context: IWorkspaceProcessContext,
     context: SensorLaunchContext,
     external_sensor: ExternalSensor,
     state: InstigatorState,
+    submit_threadpool_executor: Optional[ThreadPoolExecutor],
     sensor_debug_crash_flags: Optional[SingleInstigatorDebugCrashFlags] = None,
 ):
     instance = workspace_process_context.instance
     context.logger.info(f"Checking for new runs for sensor: {external_sensor.name}")
 
     sensor_origin = external_sensor.get_external_origin()
     repository_handle = external_sensor.handle.repository_handle
@@ -719,77 +801,56 @@
         return  # Done with run status sensors
 
     skipped_runs = []
     existing_runs_by_key = _fetch_existing_runs(
         instance, external_sensor, sensor_runtime_data.run_requests
     )
 
+    run_requests = []
+
     for raw_run_request in sensor_runtime_data.run_requests:
         if raw_run_request.stale_assets_only:
             stale_assets = resolve_stale_or_missing_assets(workspace_process_context, raw_run_request, external_sensor)  # type: ignore
             # asset selection is empty set after filtering for stale
             if len(stale_assets) == 0:
                 continue
             else:
                 run_request = raw_run_request.with_replaced_attrs(
                     asset_selection=stale_assets, stale_assets_only=False
                 )
         else:
             run_request = raw_run_request
 
-        target_data: ExternalTargetData = check.not_none(
-            external_sensor.get_target_data(run_request.job_name)
-        )
+        run_requests.append(run_request)
 
-        job_subset_selector = JobSubsetSelector(
-            location_name=code_location.name,
-            repository_name=sensor_origin.external_repository_origin.repository_name,
-            job_name=target_data.job_name,
-            op_selection=target_data.op_selection,
-            asset_selection=run_request.asset_selection,
-        )
-        external_job = code_location.get_external_job(job_subset_selector)
-        run = _get_or_create_sensor_run(
-            context,
-            instance,
-            code_location,
-            external_sensor,
-            external_job,
-            run_request,
-            target_data,
-            existing_runs_by_key,
-        )
-
-        if isinstance(run, SkippedSensorRun):
-            skipped_runs.append(run)
-            context.add_run_info(run_id=None, run_key=run_request.run_key)
-            yield
-            continue
+    submit_run_request = lambda run_request: _submit_run_request(
+        run_request,
+        workspace_process_context,
+        external_sensor,
+        code_location,
+        existing_runs_by_key,
+        context.logger,
+        sensor_debug_crash_flags,
+    )
 
-        _check_for_debug_crash(sensor_debug_crash_flags, "RUN_CREATED")
+    if submit_threadpool_executor:
+        gen_run_request_results = submit_threadpool_executor.map(submit_run_request, run_requests)
+    else:
+        gen_run_request_results = map(submit_run_request, run_requests)
 
-        error_info = None
-        try:
-            context.logger.info(f"Launching run for {external_sensor.name}")
-            instance.submit_run(run.run_id, workspace_process_context.create_request_context())
-            context.logger.info(
-                "Completed launch of run {run_id} for {sensor_name}".format(
-                    run_id=run.run_id, sensor_name=external_sensor.name
-                )
-            )
-        except Exception:
-            error_info = serializable_error_info_from_exc_info(sys.exc_info())
-            context.logger.error(
-                f"Run {run.run_id} created successfully but failed to launch: {str(error_info)}"
-            )
-        yield error_info
+    for run_request_result in gen_run_request_results:
+        yield run_request_result.error_info
 
-        _check_for_debug_crash(sensor_debug_crash_flags, "RUN_LAUNCHED")
+        run = run_request_result.run
 
-        context.add_run_info(run_id=run.run_id, run_key=run_request.run_key)
+        if isinstance(run, SkippedSensorRun):
+            skipped_runs.append(run)
+            context.add_run_info(run_id=None, run_key=run_request_result.run_key)
+        else:
+            context.add_run_info(run_id=run.run_id, run_key=run_request_result.run_key)
 
     if skipped_runs:
         run_keys = [skipped.run_key for skipped in skipped_runs]
         skipped_count = len(skipped_runs)
         context.logger.info(
             f"Skipping {skipped_count} {'run' if skipped_count == 1 else 'runs'} for sensor "
             f"{external_sensor.name} already completed with run keys: {seven.json.dumps(run_keys)}"
@@ -859,15 +920,15 @@
         run_key = tags.get(RUN_KEY_TAG)
         existing_runs[run_key] = run
 
     return existing_runs
 
 
 def _get_or_create_sensor_run(
-    context: SensorLaunchContext,
+    logger: logging.Logger,
     instance: DagsterInstance,
     code_location: CodeLocation,
     external_sensor: ExternalSensor,
     external_job: ExternalJob,
     run_request: RunRequest,
     target_data: ExternalTargetData,
     existing_runs_by_key: Mapping[str, DagsterRun],
@@ -881,21 +942,21 @@
 
     if run:
         if run.status != DagsterRunStatus.NOT_STARTED:
             # A run already exists and was launched for this run key, but the daemon must have
             # crashed before the tick could be updated
             return SkippedSensorRun(run_key=run_request.run_key, existing_run=run)
         else:
-            context.logger.info(
+            logger.info(
                 f"Run {run.run_id} already created with the run key "
                 f"`{run_request.run_key}` for {external_sensor.name}"
             )
             return run
 
-    context.logger.info(f"Creating new run for {external_sensor.name}")
+    logger.info(f"Creating new run for {external_sensor.name}")
 
     return _create_sensor_run(
         instance, code_location, external_sensor, external_job, run_request, target_data
     )
 
 
 def _create_sensor_run(
```

### Comparing `dagster-1.3.5/dagster/_daemon/types.py` & `dagster-1.3.6/dagster/_daemon/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_daemon/workspace.py` & `dagster-1.3.6/dagster/_daemon/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_generate/download.py` & `dagster-1.3.6/dagster/_generate/download.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_generate/generate.py` & `dagster-1.3.6/dagster/_generate/generate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md` & `dagster-1.3.6/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_grpc/__generated__/api_pb2.py` & `dagster-1.3.6/dagster/_grpc/__generated__/api_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,17 +61,18 @@
     b' \x01(\t"4\n\rStartRunReply\x12#\n\x1bserialized_start_run_result\x18\x01'
     b' \x01(\t"8\n\x14GetCurrentImageReply\x12 \n\x18serialized_current_image\x18\x01'
     b' \x01(\t"6\n\x13GetCurrentRunsReply\x12\x1f\n\x17serialized_current_runs\x18\x01'
     b' \x01(\t"L\n\x12\x45xternalJobRequest\x12$\n\x1cserialized_repository_origin\x18\x01'
     b" \x01(\t\x12\x10\n\x08job_name\x18\x02"
     b' \x01(\t"I\n\x10\x45xternalJobReply\x12\x1b\n\x13serialized_job_data\x18\x01'
     b" \x01(\t\x12\x18\n\x10serialized_error\x18\x02"
-    b' \x01(\t2\xd3\x0e\n\nDagsterApi\x12*\n\x04Ping\x12\x10.api.PingRequest\x1a\x0e.api.PingReply"\x00\x12/\n\tHeartbeat\x12\x10.api.PingRequest\x1a\x0e.api.PingReply"\x00\x12G\n\rStreamingPing\x12\x19.api.StreamingPingRequest\x1a\x17.api.StreamingPingEvent"\x00\x30\x01\x12\x32\n\x0bGetServerId\x12\n.api.Empty\x1a\x15.api.GetServerIdReply"\x00\x12]\n\x15\x45xecutionPlanSnapshot\x12!.api.ExecutionPlanSnapshotRequest\x1a\x1f.api.ExecutionPlanSnapshotReply"\x00\x12N\n\x10ListRepositories\x12\x1c.api.ListRepositoriesRequest\x1a\x1a.api.ListRepositoriesReply"\x00\x12`\n\x16\x45xternalPartitionNames\x12".api.ExternalPartitionNamesRequest\x1a'
+    b' \x01(\t"\x13\n\x11ReloadCodeRequest"+\n\x0fReloadCodeReply\x12\x18\n\x10serialized_error\x18\x02'
+    b' \x01(\t2\x91\x0f\n\nDagsterApi\x12*\n\x04Ping\x12\x10.api.PingRequest\x1a\x0e.api.PingReply"\x00\x12/\n\tHeartbeat\x12\x10.api.PingRequest\x1a\x0e.api.PingReply"\x00\x12G\n\rStreamingPing\x12\x19.api.StreamingPingRequest\x1a\x17.api.StreamingPingEvent"\x00\x30\x01\x12\x32\n\x0bGetServerId\x12\n.api.Empty\x1a\x15.api.GetServerIdReply"\x00\x12]\n\x15\x45xecutionPlanSnapshot\x12!.api.ExecutionPlanSnapshotRequest\x1a\x1f.api.ExecutionPlanSnapshotReply"\x00\x12N\n\x10ListRepositories\x12\x1c.api.ListRepositoriesRequest\x1a\x1a.api.ListRepositoriesReply"\x00\x12`\n\x16\x45xternalPartitionNames\x12".api.ExternalPartitionNamesRequest\x1a'
     b' .api.ExternalPartitionNamesReply"\x00\x12Z\n\x14\x45xternalNotebookData\x12'
-    b' .api.ExternalNotebookDataRequest\x1a\x1e.api.ExternalNotebookDataReply"\x00\x12\x63\n\x17\x45xternalPartitionConfig\x12#.api.ExternalPartitionConfigRequest\x1a!.api.ExternalPartitionConfigReply"\x00\x12]\n\x15\x45xternalPartitionTags\x12!.api.ExternalPartitionTagsRequest\x1a\x1f.api.ExternalPartitionTagsReply"\x00\x12t\n#ExternalPartitionSetExecutionParams\x12/.api.ExternalPartitionSetExecutionParamsRequest\x1a\x18.api.StreamingChunkEvent"\x00\x30\x01\x12x\n\x1e\x45xternalPipelineSubsetSnapshot\x12*.api.ExternalPipelineSubsetSnapshotRequest\x1a(.api.ExternalPipelineSubsetSnapshotReply"\x00\x12T\n\x12\x45xternalRepository\x12\x1e.api.ExternalRepositoryRequest\x1a\x1c.api.ExternalRepositoryReply"\x00\x12?\n\x0b\x45xternalJob\x12\x17.api.ExternalJobRequest\x1a\x15.api.ExternalJobReply"\x00\x12h\n\x1bStreamingExternalRepository\x12\x1e.api.ExternalRepositoryRequest\x1a%.api.StreamingExternalRepositoryEvent"\x00\x30\x01\x12`\n\x19\x45xternalScheduleExecution\x12%.api.ExternalScheduleExecutionRequest\x1a\x18.api.StreamingChunkEvent"\x00\x30\x01\x12\\\n\x17\x45xternalSensorExecution\x12#.api.ExternalSensorExecutionRequest\x1a\x18.api.StreamingChunkEvent"\x00\x30\x01\x12\x38\n\x0eShutdownServer\x12\n.api.Empty\x1a\x18.api.ShutdownServerReply"\x00\x12K\n\x0f\x43\x61ncelExecution\x12\x1b.api.CancelExecutionRequest\x1a\x19.api.CancelExecutionReply"\x00\x12T\n\x12\x43\x61nCancelExecution\x12\x1e.api.CanCancelExecutionRequest\x1a\x1c.api.CanCancelExecutionReply"\x00\x12\x36\n\x08StartRun\x12\x14.api.StartRunRequest\x1a\x12.api.StartRunReply"\x00\x12:\n\x0fGetCurrentImage\x12\n.api.Empty\x1a\x19.api.GetCurrentImageReply"\x00\x12\x38\n\x0eGetCurrentRuns\x12\n.api.Empty\x1a\x18.api.GetCurrentRunsReply"\x00\x62\x06proto3'
+    b' .api.ExternalNotebookDataRequest\x1a\x1e.api.ExternalNotebookDataReply"\x00\x12\x63\n\x17\x45xternalPartitionConfig\x12#.api.ExternalPartitionConfigRequest\x1a!.api.ExternalPartitionConfigReply"\x00\x12]\n\x15\x45xternalPartitionTags\x12!.api.ExternalPartitionTagsRequest\x1a\x1f.api.ExternalPartitionTagsReply"\x00\x12t\n#ExternalPartitionSetExecutionParams\x12/.api.ExternalPartitionSetExecutionParamsRequest\x1a\x18.api.StreamingChunkEvent"\x00\x30\x01\x12x\n\x1e\x45xternalPipelineSubsetSnapshot\x12*.api.ExternalPipelineSubsetSnapshotRequest\x1a(.api.ExternalPipelineSubsetSnapshotReply"\x00\x12T\n\x12\x45xternalRepository\x12\x1e.api.ExternalRepositoryRequest\x1a\x1c.api.ExternalRepositoryReply"\x00\x12?\n\x0b\x45xternalJob\x12\x17.api.ExternalJobRequest\x1a\x15.api.ExternalJobReply"\x00\x12h\n\x1bStreamingExternalRepository\x12\x1e.api.ExternalRepositoryRequest\x1a%.api.StreamingExternalRepositoryEvent"\x00\x30\x01\x12`\n\x19\x45xternalScheduleExecution\x12%.api.ExternalScheduleExecutionRequest\x1a\x18.api.StreamingChunkEvent"\x00\x30\x01\x12\\\n\x17\x45xternalSensorExecution\x12#.api.ExternalSensorExecutionRequest\x1a\x18.api.StreamingChunkEvent"\x00\x30\x01\x12\x38\n\x0eShutdownServer\x12\n.api.Empty\x1a\x18.api.ShutdownServerReply"\x00\x12K\n\x0f\x43\x61ncelExecution\x12\x1b.api.CancelExecutionRequest\x1a\x19.api.CancelExecutionReply"\x00\x12T\n\x12\x43\x61nCancelExecution\x12\x1e.api.CanCancelExecutionRequest\x1a\x1c.api.CanCancelExecutionReply"\x00\x12\x36\n\x08StartRun\x12\x14.api.StartRunRequest\x1a\x12.api.StartRunReply"\x00\x12:\n\x0fGetCurrentImage\x12\n.api.Empty\x1a\x19.api.GetCurrentImageReply"\x00\x12\x38\n\x0eGetCurrentRuns\x12\n.api.Empty\x1a\x18.api.GetCurrentRunsReply"\x00\x12<\n\nReloadCode\x12\x16.api.ReloadCodeRequest\x1a\x14.api.ReloadCodeReply"\x00\x62\x06proto3'
 )
 
 
 _EMPTY = DESCRIPTOR.message_types_by_name["Empty"]
 _PINGREQUEST = DESCRIPTOR.message_types_by_name["PingRequest"]
 _PINGREPLY = DESCRIPTOR.message_types_by_name["PingReply"]
 _STREAMINGPINGREQUEST = DESCRIPTOR.message_types_by_name["StreamingPingRequest"]
@@ -115,14 +116,16 @@
 _CANCANCELEXECUTIONREPLY = DESCRIPTOR.message_types_by_name["CanCancelExecutionReply"]
 _STARTRUNREQUEST = DESCRIPTOR.message_types_by_name["StartRunRequest"]
 _STARTRUNREPLY = DESCRIPTOR.message_types_by_name["StartRunReply"]
 _GETCURRENTIMAGEREPLY = DESCRIPTOR.message_types_by_name["GetCurrentImageReply"]
 _GETCURRENTRUNSREPLY = DESCRIPTOR.message_types_by_name["GetCurrentRunsReply"]
 _EXTERNALJOBREQUEST = DESCRIPTOR.message_types_by_name["ExternalJobRequest"]
 _EXTERNALJOBREPLY = DESCRIPTOR.message_types_by_name["ExternalJobReply"]
+_RELOADCODEREQUEST = DESCRIPTOR.message_types_by_name["ReloadCodeRequest"]
+_RELOADCODEREPLY = DESCRIPTOR.message_types_by_name["ReloadCodeReply"]
 Empty = _reflection.GeneratedProtocolMessageType(
     "Empty",
     (_message.Message,),
     {
         "DESCRIPTOR": _EMPTY,
         "__module__": "api_pb2"
         # @@protoc_insertion_point(class_scope:api.Empty)
@@ -533,14 +536,36 @@
         "DESCRIPTOR": _EXTERNALJOBREPLY,
         "__module__": "api_pb2"
         # @@protoc_insertion_point(class_scope:api.ExternalJobReply)
     },
 )
 _sym_db.RegisterMessage(ExternalJobReply)
 
+ReloadCodeRequest = _reflection.GeneratedProtocolMessageType(
+    "ReloadCodeRequest",
+    (_message.Message,),
+    {
+        "DESCRIPTOR": _RELOADCODEREQUEST,
+        "__module__": "api_pb2"
+        # @@protoc_insertion_point(class_scope:api.ReloadCodeRequest)
+    },
+)
+_sym_db.RegisterMessage(ReloadCodeRequest)
+
+ReloadCodeReply = _reflection.GeneratedProtocolMessageType(
+    "ReloadCodeReply",
+    (_message.Message,),
+    {
+        "DESCRIPTOR": _RELOADCODEREPLY,
+        "__module__": "api_pb2"
+        # @@protoc_insertion_point(class_scope:api.ReloadCodeReply)
+    },
+)
+_sym_db.RegisterMessage(ReloadCodeReply)
+
 _DAGSTERAPI = DESCRIPTOR.services_by_name["DagsterApi"]
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     _EMPTY._serialized_start = 18
     _EMPTY._serialized_end = 25
     _PINGREQUEST._serialized_start = 27
     _PINGREQUEST._serialized_end = 54
@@ -612,10 +637,14 @@
     _GETCURRENTIMAGEREPLY._serialized_end = 2494
     _GETCURRENTRUNSREPLY._serialized_start = 2496
     _GETCURRENTRUNSREPLY._serialized_end = 2550
     _EXTERNALJOBREQUEST._serialized_start = 2552
     _EXTERNALJOBREQUEST._serialized_end = 2628
     _EXTERNALJOBREPLY._serialized_start = 2630
     _EXTERNALJOBREPLY._serialized_end = 2703
-    _DAGSTERAPI._serialized_start = 2706
-    _DAGSTERAPI._serialized_end = 4581
+    _RELOADCODEREQUEST._serialized_start = 2705
+    _RELOADCODEREQUEST._serialized_end = 2724
+    _RELOADCODEREPLY._serialized_start = 2726
+    _RELOADCODEREPLY._serialized_end = 2769
+    _DAGSTERAPI._serialized_start = 2772
+    _DAGSTERAPI._serialized_end = 4709
 # @@protoc_insertion_point(module_scope)
```

### Comparing `dagster-1.3.5/dagster/_grpc/__generated__/api_pb2_grpc.py` & `dagster-1.3.6/dagster/_grpc/__generated__/api_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,19 @@
             response_deserializer=api__pb2.GetCurrentImageReply.FromString,
         )
         self.GetCurrentRuns = channel.unary_unary(
             "/api.DagsterApi/GetCurrentRuns",
             request_serializer=api__pb2.Empty.SerializeToString,
             response_deserializer=api__pb2.GetCurrentRunsReply.FromString,
         )
+        self.ReloadCode = channel.unary_unary(
+            "/api.DagsterApi/ReloadCode",
+            request_serializer=api__pb2.ReloadCodeRequest.SerializeToString,
+            response_deserializer=api__pb2.ReloadCodeReply.FromString,
+        )
 
 
 class DagsterApiServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def Ping(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -274,14 +279,20 @@
 
     def GetCurrentRuns(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
+    def ReloadCode(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details("Method not implemented!")
+        raise NotImplementedError("Method not implemented!")
+
 
 def add_DagsterApiServicer_to_server(servicer, server):
     rpc_method_handlers = {
         "Ping": grpc.unary_unary_rpc_method_handler(
             servicer.Ping,
             request_deserializer=api__pb2.PingRequest.FromString,
             response_serializer=api__pb2.PingReply.SerializeToString,
@@ -392,14 +403,19 @@
             response_serializer=api__pb2.GetCurrentImageReply.SerializeToString,
         ),
         "GetCurrentRuns": grpc.unary_unary_rpc_method_handler(
             servicer.GetCurrentRuns,
             request_deserializer=api__pb2.Empty.FromString,
             response_serializer=api__pb2.GetCurrentRunsReply.SerializeToString,
         ),
+        "ReloadCode": grpc.unary_unary_rpc_method_handler(
+            servicer.ReloadCode,
+            request_deserializer=api__pb2.ReloadCodeRequest.FromString,
+            response_serializer=api__pb2.ReloadCodeReply.SerializeToString,
+        ),
     }
     generic_handler = grpc.method_handlers_generic_handler("api.DagsterApi", rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
 # This class is part of an EXPERIMENTAL API.
 class DagsterApi(object):
@@ -1065,9 +1081,38 @@
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
+            metadata,
+        )
+
+    @staticmethod
+    def ReloadCode(
+        request,
+        target,
+        options=(),
+        channel_credentials=None,
+        call_credentials=None,
+        insecure=False,
+        compression=None,
+        wait_for_ready=None,
+        timeout=None,
+        metadata=None,
+    ):
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            "/api.DagsterApi/ReloadCode",
+            api__pb2.ReloadCodeRequest.SerializeToString,
+            api__pb2.ReloadCodeReply.FromString,
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
             metadata,
         )
```

### Comparing `dagster-1.3.5/dagster/_grpc/__init__.py` & `dagster-1.3.6/dagster/_grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_grpc/client.py` & `dagster-1.3.6/dagster/_grpc/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,14 +292,17 @@
             "ExternalPipelineSubsetSnapshot",
             api_pb2.ExternalPipelineSubsetSnapshotRequest,
             serialized_pipeline_subset_snapshot_args=serialize_value(pipeline_subset_snapshot_args),
         )
 
         return res.serialized_external_pipeline_subset_result
 
+    def reload_code(self, timeout: int):
+        return self._query("ReloadCode", api_pb2.ReloadCodeRequest, timeout=timeout)
+
     def external_repository(
         self,
         external_repository_origin: ExternalRepositoryOrigin,
         defer_snapshots: bool = False,
     ):
         check.inst_param(
             external_repository_origin,
```

### Comparing `dagster-1.3.5/dagster/_grpc/compile.py` & `dagster-1.3.6/dagster/_grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_grpc/impl.py` & `dagster-1.3.6/dagster/_grpc/impl.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_grpc/protos/api.proto` & `dagster-1.3.6/dagster/_grpc/protos/api.proto`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
   rpc ExternalSensorExecution (ExternalSensorExecutionRequest) returns (stream StreamingChunkEvent) {}
   rpc ShutdownServer (Empty) returns (ShutdownServerReply) {}
   rpc CancelExecution (CancelExecutionRequest) returns (CancelExecutionReply) {}
   rpc CanCancelExecution (CanCancelExecutionRequest) returns (CanCancelExecutionReply) {}
   rpc StartRun (StartRunRequest) returns (StartRunReply) {}
   rpc GetCurrentImage (Empty) returns (GetCurrentImageReply) {}
   rpc GetCurrentRuns (Empty) returns (GetCurrentRunsReply) {}
+  rpc ReloadCode (ReloadCodeRequest) returns (ReloadCodeReply) {}
 }
 
 message Empty {}
 
 message PingRequest {
   string echo = 1;
 }
@@ -181,7 +182,14 @@
   string job_name = 2;
 }
 
 message ExternalJobReply {
   string serialized_job_data = 1;
   string serialized_error = 2;
 }
+
+message ReloadCodeRequest {
+}
+
+message ReloadCodeReply {
+  string serialized_error = 2;
+}
```

### Comparing `dagster-1.3.5/dagster/_grpc/server.py` & `dagster-1.3.6/dagster/_grpc/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+import json
+import logging
 import math
 import multiprocessing
 import os
 import queue
 import sys
 import threading
 import time
@@ -193,14 +195,15 @@
 class DagsterApiServer(DagsterApiServicer):
     # The loadable_target_origin is currently Noneable to support instaniating a server.
     # This helps us test the ping methods, and incrementally migrate each method to
     # the target passed in here instead of passing in a target in the argument.
     def __init__(
         self,
         server_termination_event: ThreadingEventType,
+        logger: logging.Logger,
         loadable_target_origin: Optional[LoadableTargetOrigin] = None,
         heartbeat: bool = False,
         heartbeat_timeout: int = 30,
         lazy_load_user_code: bool = False,
         fixed_server_id: Optional[str] = None,
         entry_point: Optional[Sequence[str]] = None,
         container_image: Optional[str] = None,
@@ -217,14 +220,15 @@
 
         self._server_termination_event = check.inst_param(
             server_termination_event, "server_termination_event", ThreadingEventType
         )
         self._loadable_target_origin = check.opt_inst_param(
             loadable_target_origin, "loadable_target_origin", LoadableTargetOrigin
         )
+        self._logger = logger
 
         self._mp_ctx = multiprocessing.get_context("spawn")
 
         # Each server is initialized with a unique UUID. This UUID is used by clients to track when
         # servers are replaced and is used for cache invalidation and reloading.
         self._server_id = check.opt_str_param(fixed_server_id, "fixed_server_id", str(uuid.uuid4()))
 
@@ -273,14 +277,15 @@
                 self._container_image,
             )
         except Exception:
             if not lazy_load_user_code:
                 raise
             self._loaded_repositories = None
             self._serializable_load_error = serializable_error_info_from_exc_info(sys.exc_info())
+            self._logger.exception("Error while importing code")
 
         self.__last_heartbeat_time = time.time()
         if heartbeat:
             self.__heartbeat_thread: Optional[threading.Thread] = threading.Thread(
                 target=self._heartbeat_thread,
                 args=(heartbeat_timeout,),
                 name="grpc-server-heartbeat",
@@ -294,14 +299,16 @@
             target=self._cleanup_thread, args=(), name="grpc-server-cleanup"
         )
         self.__cleanup_thread.daemon = True
 
         self.__cleanup_thread.start()
 
     def cleanup(self) -> None:
+        # In case ShutdownServer was not called
+        self._shutdown_once_executions_finish_event.set()
         if self.__heartbeat_thread:
             self.__heartbeat_thread.join()
         self.__cleanup_thread.join()
 
     def _heartbeat_thread(self, heartbeat_timeout: float) -> None:
         while True:
             self._shutdown_once_executions_finish_event.wait(heartbeat_timeout)
@@ -696,14 +703,15 @@
             self._shutdown_once_executions_finish_event.set()
             return api_pb2.ShutdownServerReply(
                 serialized_shutdown_server_result=serialize_value(
                     ShutdownServerResult(success=True, serializable_error_info=None)
                 )
             )
         except:
+            self._logger.exception("Failed to shut down server")
             return api_pb2.ShutdownServerReply(
                 serialized_shutdown_server_result=serialize_value(
                     ShutdownServerResult(
                         success=False,
                         serializable_error_info=serializable_error_info_from_exc_info(
                             sys.exc_info()
                         ),
@@ -988,22 +996,21 @@
         server_termination_thread = threading.Thread(
             target=server_termination_target,
             args=[self._server_termination_event, self.server],
             name="grpc-server-termination",
         )
 
         server_termination_thread.daemon = True
-
         server_termination_thread.start()
 
-        self.server.wait_for_termination()
-
-        server_termination_thread.join()
-
-        self._api_servicer.cleanup()
+        try:
+            self.server.wait_for_termination()
+        finally:
+            self._api_servicer.cleanup()
+            server_termination_thread.join()
 
 
 class CouldNotStartServerProcess(Exception):
     def __init__(self, port=None, socket=None):
         super(CouldNotStartServerProcess, self).__init__(
             "Could not start server with "
             + (f"port {port}" if port is not None else f"socket {socket}")
@@ -1034,27 +1041,30 @@
                 f" with the command: \"{' '.join(subprocess_args)}\""
             )
 
         sleep(0.1)
 
 
 def open_server_process(
-    instance_ref: InstanceRef,
+    instance_ref: Optional[InstanceRef],
     port: Optional[int],
     socket: Optional[str],
     location_name: Optional[str] = None,
     loadable_target_origin: Optional[LoadableTargetOrigin] = None,
     max_workers: Optional[int] = None,
     heartbeat: bool = False,
     heartbeat_timeout: int = 30,
     fixed_server_id: Optional[str] = None,
     startup_timeout: int = 20,
     cwd: Optional[str] = None,
     log_level: str = "INFO",
     env: Optional[Dict[str, str]] = None,
+    inject_env_vars_from_instance: bool = True,
+    container_image: Optional[str] = None,
+    container_context: Optional[dict[str, Any]] = None,
 ):
     check.invariant((port or socket) and not (port and socket), "Set only port or socket")
     check.opt_inst_param(loadable_target_origin, "loadable_target_origin", LoadableTargetOrigin)
     check.opt_int_param(max_workers, "max_workers")
 
     from dagster._core.test_utils import get_mocked_system_timezone
 
@@ -1072,17 +1082,19 @@
         *(["--heartbeat"] if heartbeat else []),
         *(["--heartbeat-timeout", str(heartbeat_timeout)] if heartbeat_timeout else []),
         *(["--fixed-server-id", fixed_server_id] if fixed_server_id else []),
         *(["--override-system-timezone", mocked_system_timezone] if mocked_system_timezone else []),
         *(["--log-level", log_level]),
         # only use the Python environment if it has been explicitly set in the workspace,
         *(["--use-python-environment-entry-point"] if executable_path else []),
-        *(["--inject-env-vars-from-instance"]),
-        *(["--instance-ref", serialize_value(instance_ref)]),
+        *(["--inject-env-vars-from-instance"] if inject_env_vars_from_instance else []),
+        *(["--instance-ref", serialize_value(instance_ref)] if instance_ref else []),
         *(["--location-name", location_name] if location_name else []),
+        *(["--container-image", container_image] if container_image else []),
+        *(["--container-context", json.dumps(container_context)] if container_context else []),
     ]
 
     if loadable_target_origin:
         subprocess_args += loadable_target_origin.get_cli_args()
 
     server_process = open_ipc_subprocess(subprocess_args, cwd=cwd, env=env)
 
@@ -1101,73 +1113,52 @@
             server_process.terminate()
         raise
 
     return server_process
 
 
 def _open_server_process_on_dynamic_port(
-    instance_ref: InstanceRef,
-    location_name: Optional[str] = None,
     max_retries: int = 10,
-    loadable_target_origin: Optional[LoadableTargetOrigin] = None,
-    max_workers: Optional[int] = None,
-    heartbeat: bool = False,
-    heartbeat_timeout: int = 30,
-    fixed_server_id: Optional[str] = None,
-    startup_timeout: int = 20,
-    cwd: Optional[str] = None,
-    log_level: str = "INFO",
-    env: Optional[Dict[str, str]] = None,
+    **kwargs,
 ) -> Tuple[Optional[Popen[str]], Optional[int]]:
     server_process = None
     retries = 0
     port = None
     while server_process is None and retries < max_retries:
         port = find_free_port()
         try:
-            server_process = open_server_process(
-                instance_ref=instance_ref,
-                location_name=location_name,
-                port=port,
-                socket=None,
-                loadable_target_origin=loadable_target_origin,
-                max_workers=max_workers,
-                heartbeat=heartbeat,
-                heartbeat_timeout=heartbeat_timeout,
-                fixed_server_id=fixed_server_id,
-                startup_timeout=startup_timeout,
-                cwd=cwd,
-                log_level=log_level,
-                env=env,
-            )
+            server_process = open_server_process(port=port, socket=None, **kwargs)
         except CouldNotBindGrpcServerToAddress:
             pass
 
         retries += 1
 
     return server_process, port
 
 
 class GrpcServerProcess:
     def __init__(
         self,
-        instance_ref: InstanceRef,
+        instance_ref: Optional[InstanceRef],
         location_name: Optional[str] = None,
         loadable_target_origin: Optional[LoadableTargetOrigin] = None,
         force_port: bool = False,
         max_retries: int = 10,
         max_workers: Optional[int] = None,
         heartbeat: bool = False,
         heartbeat_timeout: int = 30,
         fixed_server_id: Optional[str] = None,
         startup_timeout: int = 20,
         cwd: Optional[str] = None,
         log_level: str = "INFO",
         env: Optional[Dict[str, str]] = None,
         wait_on_exit=False,
+        inject_env_vars_from_instance: bool = True,
+        container_image: Optional[str] = None,
+        container_context: Optional[Dict[str, Any]] = None,
     ):
         self.port = None
         self.socket = None
         self._waited = False
         self._shutdown = False
         self._heartbeat = heartbeat
         self._server_process = None
@@ -1200,14 +1191,17 @@
                 heartbeat=heartbeat,
                 heartbeat_timeout=heartbeat_timeout,
                 fixed_server_id=fixed_server_id,
                 startup_timeout=startup_timeout,
                 cwd=cwd,
                 log_level=log_level,
                 env=env,
+                inject_env_vars_from_instance=inject_env_vars_from_instance,
+                container_image=container_image,
+                container_context=container_context,
             )
         else:
             self.socket = safe_tempfile_path_unmanaged()
 
             server_process = open_server_process(
                 instance_ref=instance_ref,
                 location_name=location_name,
@@ -1218,14 +1212,17 @@
                 heartbeat=heartbeat,
                 heartbeat_timeout=heartbeat_timeout,
                 fixed_server_id=fixed_server_id,
                 startup_timeout=startup_timeout,
                 cwd=cwd,
                 log_level=log_level,
                 env=env,
+                inject_env_vars_from_instance=inject_env_vars_from_instance,
+                container_image=container_image,
+                container_context=container_context,
             )
 
         if server_process is None:
             raise CouldNotStartServerProcess(port=self.port, socket=self.socket)
         else:
             self._server_process = server_process
```

### Comparing `dagster-1.3.5/dagster/_grpc/server_watcher.py` & `dagster-1.3.6/dagster/_grpc/server_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_grpc/types.py` & `dagster-1.3.6/dagster/_grpc/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_grpc/utils.py` & `dagster-1.3.6/dagster/_grpc/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_loggers/__init__.py` & `dagster-1.3.6/dagster/_loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_module_alias_map.py` & `dagster-1.3.6/dagster/_module_alias_map.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_scheduler/scheduler.py` & `dagster-1.3.6/dagster/_scheduler/scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import sys
 import threading
 import time
 from collections import defaultdict
 from concurrent.futures import Future, ThreadPoolExecutor
 from contextlib import ExitStack
-from typing import TYPE_CHECKING, Dict, List, Mapping, Optional, cast
+from typing import TYPE_CHECKING, Dict, List, Mapping, NamedTuple, Optional, cast
 
 import pendulum
 
 import dagster._check as check
 from dagster._core.definitions.run_request import RunRequest
 from dagster._core.definitions.schedule_definition import DefaultScheduleStatus
 from dagster._core.definitions.selector import JobSubsetSelector
@@ -34,15 +34,15 @@
 from dagster._core.storage.dagster_run import DagsterRun, DagsterRunStatus, RunsFilter
 from dagster._core.storage.tags import RUN_KEY_TAG, SCHEDULED_EXECUTION_TIME_TAG
 from dagster._core.telemetry import SCHEDULED_RUN_CREATED, hash_name, log_action
 from dagster._core.workspace.context import IWorkspaceProcessContext
 from dagster._scheduler.stale import resolve_stale_or_missing_assets
 from dagster._seven.compat.pendulum import to_timezone
 from dagster._utils import DebugCrashFlags, SingleInstigatorDebugCrashFlags
-from dagster._utils.error import serializable_error_info_from_exc_info
+from dagster._utils.error import SerializableErrorInfo, serializable_error_info_from_exc_info
 from dagster._utils.log import default_date_format_string
 from dagster._utils.merger import merge_dicts
 
 if TYPE_CHECKING:
     from pendulum.datetime import DateTime
 
     from dagster._daemon.daemon import DaemonIterator
@@ -121,25 +121,34 @@
     max_catchup_runs: int,
     max_tick_retries: int,
     shutdown_event: threading.Event,
 ) -> "DaemonIterator":
     schedule_state_lock = threading.Lock()
     scheduler_run_futures: Dict[str, Future] = {}
 
+    submit_threadpool_executor = None
+    threadpool_executor = None
+
     with ExitStack() as stack:
         settings = workspace_process_context.instance.get_settings("schedules")
         if settings.get("use_threads"):
             threadpool_executor = stack.enter_context(
                 ThreadPoolExecutor(
                     max_workers=settings.get("num_workers"),
                     thread_name_prefix="schedule_daemon_worker",
                 )
             )
-        else:
-            threadpool_executor = None
+            num_submit_workers = settings.get("num_submit_workers")
+            if num_submit_workers:
+                submit_threadpool_executor = stack.enter_context(
+                    ThreadPoolExecutor(
+                        max_workers=settings.get("num_submit_workers"),
+                        thread_name_prefix="schedule_submit_worker",
+                    )
+                )
 
         last_verbose_time = None
         while True:
             start_time = pendulum.now("UTC").timestamp()
             end_datetime_utc = pendulum.now("UTC")
 
             # occasionally enable verbose logging (doing it always would be too much)
@@ -147,14 +156,15 @@
                 last_verbose_time is None or start_time - last_verbose_time > VERBOSE_LOGS_INTERVAL
             )
             yield from launch_scheduled_runs(
                 workspace_process_context,
                 logger,
                 end_datetime_utc=end_datetime_utc,
                 threadpool_executor=threadpool_executor,
+                submit_threadpool_executor=submit_threadpool_executor,
                 scheduler_run_futures=scheduler_run_futures,
                 schedule_state_lock=schedule_state_lock,
                 max_catchup_runs=max_catchup_runs,
                 max_tick_retries=max_tick_retries,
                 log_verbose_checks=verbose_logs_iteration,
             )
             yield
@@ -173,14 +183,15 @@
 
 
 def launch_scheduled_runs(
     workspace_process_context: IWorkspaceProcessContext,
     logger: logging.Logger,
     end_datetime_utc: "DateTime",
     threadpool_executor: Optional[ThreadPoolExecutor] = None,
+    submit_threadpool_executor: Optional[ThreadPoolExecutor] = None,
     scheduler_run_futures: Optional[Dict[str, Future]] = None,
     schedule_state_lock: Optional[threading.Lock] = None,
     max_catchup_runs: int = DEFAULT_MAX_CATCHUP_RUNS,
     max_tick_retries: int = 0,
     debug_crash_flags: Optional[DebugCrashFlags] = None,
     log_verbose_checks: bool = True,
 ) -> "DaemonIterator":
@@ -336,14 +347,15 @@
                     schedule_state_lock,
                     end_datetime_utc,
                     max_catchup_runs,
                     max_tick_retries,
                     tick_retention_settings,
                     schedule_debug_crash_flags,
                     log_verbose_checks=log_verbose_checks,
+                    submit_threadpool_executor=submit_threadpool_executor,
                 )
                 scheduler_run_futures[external_schedule.selector_id] = future
                 yield
 
             else:
                 # evaluate the schedules in a loop, synchronously, yielding to allow the schedule daemon to
                 # heartbeat
@@ -355,14 +367,15 @@
                     schedule_state_lock,
                     end_datetime_utc,
                     max_catchup_runs,
                     max_tick_retries,
                     tick_retention_settings,
                     schedule_debug_crash_flags,
                     log_verbose_checks=log_verbose_checks,
+                    submit_threadpool_executor=None,
                 )
         except Exception:
             error_info = serializable_error_info_from_exc_info(sys.exc_info())
             logger.exception(f"Scheduler caught an error for schedule {external_schedule.name}")
         yield error_info
 
 
@@ -374,14 +387,15 @@
     schedule_state_lock: threading.Lock,
     end_datetime_utc: datetime.datetime,
     max_catchup_runs: int,
     max_tick_retries: int,
     tick_retention_settings: Mapping[TickStatus, int],
     schedule_debug_crash_flags: Optional[SingleInstigatorDebugCrashFlags],
     log_verbose_checks: bool,
+    submit_threadpool_executor: Optional[ThreadPoolExecutor],
 ) -> None:
     # evaluate the tick immediately, but from within a thread.  The main thread should be able to
     # heartbeat to keep the daemon alive
     list(
         launch_scheduled_runs_for_schedule_iterator(
             workspace_process_context,
             logger,
@@ -390,14 +404,15 @@
             schedule_state_lock,
             end_datetime_utc,
             max_catchup_runs,
             max_tick_retries,
             tick_retention_settings,
             schedule_debug_crash_flags,
             log_verbose_checks,
+            submit_threadpool_executor=submit_threadpool_executor,
         )
     )
 
 
 def launch_scheduled_runs_for_schedule_iterator(
     workspace_process_context: IWorkspaceProcessContext,
     logger: logging.Logger,
@@ -406,14 +421,15 @@
     schedule_state_lock: threading.Lock,
     end_datetime_utc: datetime.datetime,
     max_catchup_runs: int,
     max_tick_retries: int,
     tick_retention_settings: Mapping[TickStatus, int],
     schedule_debug_crash_flags: Optional[SingleInstigatorDebugCrashFlags],
     log_verbose_checks: bool,
+    submit_threadpool_executor: Optional[ThreadPoolExecutor],
 ) -> "DaemonIterator":
     schedule_state = check.inst_param(schedule_state, "schedule_state", InstigatorState)
     end_datetime_utc = check.inst_param(end_datetime_utc, "end_datetime_utc", datetime.datetime)
     instance = workspace_process_context.instance
 
     with schedule_state_lock:
         instigator_origin_id = external_schedule.get_external_origin_id()
@@ -515,14 +531,15 @@
 
                 yield from _schedule_runs_at_time(
                     workspace_process_context,
                     logger,
                     external_schedule,
                     schedule_time,
                     tick_context,
+                    submit_threadpool_executor,
                     schedule_debug_crash_flags,
                 )
             except Exception as e:
                 if isinstance(e, DagsterUserCodeUnreachableError):
                     try:
                         raise DagsterSchedulerError(
                             f"Unable to reach the user code server for schedule {schedule_name}."
@@ -568,23 +585,99 @@
         return
 
     os.kill(os.getpid(), kill_signal)
     time.sleep(10)
     raise Exception("Process didn't terminate after sending crash signal")
 
 
+class SubmitRunRequestResult(NamedTuple):
+    run_key: Optional[str]
+    error_info: Optional[SerializableErrorInfo]
+    existing_run: Optional[DagsterRun]
+    submitted_run: Optional[DagsterRun]
+
+
+def _submit_run_request(
+    run_request: RunRequest,
+    workspace_process_context: IWorkspaceProcessContext,
+    external_schedule: ExternalSchedule,
+    schedule_time: datetime.datetime,
+    code_location: CodeLocation,
+    logger,
+    debug_crash_flags,
+) -> SubmitRunRequestResult:
+    instance = workspace_process_context.instance
+    schedule_origin = external_schedule.get_external_origin()
+
+    run = _get_existing_run_for_request(instance, external_schedule, schedule_time, run_request)
+    if run:
+        if run.status != DagsterRunStatus.NOT_STARTED:
+            # A run already exists and was launched for this time period,
+            # but the scheduler must have crashed or errored before the tick could be put
+            # into a SUCCESS state
+            logger.info(
+                f"Run {run.run_id} already completed for this execution of {external_schedule.name}"
+            )
+            return SubmitRunRequestResult(
+                run_key=run_request.run_key, error_info=None, existing_run=run, submitted_run=None
+            )
+        else:
+            logger.info(
+                f"Run {run.run_id} already created for this execution of {external_schedule.name}"
+            )
+    else:
+        job_subset_selector = JobSubsetSelector(
+            location_name=schedule_origin.external_repository_origin.code_location_origin.location_name,
+            repository_name=schedule_origin.external_repository_origin.repository_name,
+            job_name=external_schedule.job_name,
+            op_selection=external_schedule.op_selection,
+            asset_selection=run_request.asset_selection,
+        )
+        external_job = code_location.get_external_job(job_subset_selector)
+
+        run = _create_scheduler_run(
+            instance,
+            schedule_time,
+            code_location,
+            external_schedule,
+            external_job,
+            run_request,
+        )
+
+    _check_for_debug_crash(debug_crash_flags, "RUN_CREATED")
+
+    error_info = None
+
+    if run.status != DagsterRunStatus.FAILURE:
+        try:
+            instance.submit_run(run.run_id, workspace_process_context.create_request_context())
+            logger.info(
+                f"Completed scheduled launch of run {run.run_id} for {external_schedule.name}"
+            )
+        except Exception:
+            error_info = serializable_error_info_from_exc_info(sys.exc_info())
+            logger.exception(f"Run {run.run_id} created successfully but failed to launch")
+
+    return SubmitRunRequestResult(
+        run_key=run_request.run_key,
+        error_info=error_info,
+        existing_run=None,
+        submitted_run=run,
+    )
+
+
 def _schedule_runs_at_time(
     workspace_process_context: IWorkspaceProcessContext,
     logger: logging.Logger,
     external_schedule: ExternalSchedule,
     schedule_time: datetime.datetime,
     tick_context: _ScheduleLaunchContext,
+    submit_threadpool_executor: Optional[ThreadPoolExecutor],
     debug_crash_flags: Optional[SingleInstigatorDebugCrashFlags] = None,
 ) -> "DaemonIterator":
-    schedule_name = external_schedule.name
     instance = workspace_process_context.instance
     schedule_origin = external_schedule.get_external_origin()
     repository_handle = external_schedule.handle.repository_handle
 
     code_location = workspace_process_context.create_request_context().get_code_location(
         schedule_origin.external_repository_origin.code_location_origin.location_name
     )
@@ -610,80 +703,58 @@
 
         # Update tick to skipped state and return
         tick_context.update_state(
             TickStatus.SKIPPED, skip_reason=schedule_execution_data.skip_message
         )
         return
 
+    run_requests = []
+
     for raw_run_request in schedule_execution_data.run_requests:
         if raw_run_request.stale_assets_only:
             stale_assets = resolve_stale_or_missing_assets(workspace_process_context, raw_run_request, external_schedule)  # type: ignore
             # asset selection is empty set after filtering for stale
             if len(stale_assets) == 0:
                 continue
             else:
                 run_request = raw_run_request.with_replaced_attrs(
                     asset_selection=stale_assets, stale_assets_only=False
                 )
         else:
             run_request = raw_run_request
 
-        job_subset_selector = JobSubsetSelector(
-            location_name=schedule_origin.external_repository_origin.code_location_origin.location_name,
-            repository_name=schedule_origin.external_repository_origin.repository_name,
-            job_name=external_schedule.job_name,
-            op_selection=external_schedule.op_selection,
-            asset_selection=run_request.asset_selection,
-        )
-        external_job = code_location.get_external_job(job_subset_selector)
+        run_requests.append(run_request)
 
-        run = _get_existing_run_for_request(instance, external_schedule, schedule_time, run_request)
-        if run:
-            if run.status != DagsterRunStatus.NOT_STARTED:
-                # A run already exists and was launched for this time period,
-                # but the scheduler must have crashed or errored before the tick could be put
-                # into a SUCCESS state
+    submit_run_request = lambda run_request: _submit_run_request(
+        run_request,
+        workspace_process_context,
+        external_schedule,
+        schedule_time,
+        code_location,
+        logger,
+        debug_crash_flags,
+    )
 
-                logger.info(
-                    f"Run {run.run_id} already completed for this execution of"
-                    f" {external_schedule.name}"
-                )
-                tick_context.add_run_info(run_id=run.run_id, run_key=run_request.run_key)
-                yield None
-                continue
-            else:
-                logger.info(
-                    f"Run {run.run_id} already created for this execution of"
-                    f" {external_schedule.name}"
-                )
-        else:
-            run = _create_scheduler_run(
-                instance,
-                schedule_time,
-                code_location,
-                external_schedule,
-                external_job,
-                run_request,
-            )
+    if submit_threadpool_executor:
+        gen_run_request_results = submit_threadpool_executor.map(submit_run_request, run_requests)
+    else:
+        gen_run_request_results = map(submit_run_request, run_requests)
 
-        _check_for_debug_crash(debug_crash_flags, "RUN_CREATED")
+    for run_request_result in gen_run_request_results:
+        yield run_request_result.error_info
 
-        if run.status != DagsterRunStatus.FAILURE:
-            try:
-                instance.submit_run(run.run_id, workspace_process_context.create_request_context())
-                logger.info(f"Completed scheduled launch of run {run.run_id} for {schedule_name}")
-            except Exception:
-                error_info = serializable_error_info_from_exc_info(sys.exc_info())
-                logger.exception(f"Run {run.run_id} created successfully but failed to launch")
-                yield error_info
-
-        _check_for_debug_crash(debug_crash_flags, "RUN_LAUNCHED")
-        tick_context.add_run_info(run_id=run.run_id, run_key=run_request.run_key)
-        _check_for_debug_crash(debug_crash_flags, "RUN_ADDED")
-        yield
+        if run_request_result.existing_run:
+            tick_context.add_run_info(
+                run_id=run_request_result.existing_run.run_id, run_key=run_request_result.run_key
+            )
+        else:
+            run = check.not_none(run_request_result.submitted_run)
+            _check_for_debug_crash(debug_crash_flags, "RUN_LAUNCHED")
+            tick_context.add_run_info(run_id=run.run_id, run_key=run_request_result.run_key)
+            _check_for_debug_crash(debug_crash_flags, "RUN_ADDED")
 
     _check_for_debug_crash(debug_crash_flags, "TICK_SUCCESS")
     tick_context.update_state(TickStatus.SUCCESS)
 
 
 def _get_existing_run_for_request(
     instance: DagsterInstance,
```

### Comparing `dagster-1.3.5/dagster/_scheduler/stale.py` & `dagster-1.3.6/dagster/_scheduler/stale.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_serdes/__init__.py` & `dagster-1.3.6/dagster/_serdes/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_serdes/config_class.py` & `dagster-1.3.6/dagster/_serdes/config_class.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_serdes/ipc.py` & `dagster-1.3.6/dagster/_serdes/ipc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_serdes/serdes.py` & `dagster-1.3.6/dagster/_serdes/serdes.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_serdes/utils.py` & `dagster-1.3.6/dagster/_serdes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_seven/__init__.py` & `dagster-1.3.6/dagster/_seven/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_seven/abc.py` & `dagster-1.3.6/dagster/_seven/abc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_seven/compat/pendulum.py` & `dagster-1.3.6/dagster/_seven/compat/pendulum.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_utils/__init__.py` & `dagster-1.3.6/dagster/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_utils/alert.py` & `dagster-1.3.6/dagster/_utils/alert.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_utils/backcompat.py` & `dagster-1.3.6/dagster/_utils/backcompat.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_utils/backoff.py` & `dagster-1.3.6/dagster/_utils/backoff.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_utils/cached_method.py` & `dagster-1.3.6/dagster/_utils/cached_method.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_utils/caching_instance_queryer.py` & `dagster-1.3.6/dagster/_utils/caching_instance_queryer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_utils/dagster_type.py` & `dagster-1.3.6/dagster/_utils/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_utils/error.py` & `dagster-1.3.6/dagster/_utils/error.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_utils/external.py` & `dagster-1.3.6/dagster/_utils/external.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_utils/forked_pdb.py` & `dagster-1.3.6/dagster/_utils/forked_pdb.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_utils/hosted_user_process.py` & `dagster-1.3.6/dagster/_utils/hosted_user_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_utils/indenting_printer.py` & `dagster-1.3.6/dagster/_utils/indenting_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_utils/interrupts.py` & `dagster-1.3.6/dagster/_utils/interrupts.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_utils/log.py` & `dagster-1.3.6/dagster/_utils/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_utils/merger.py` & `dagster-1.3.6/dagster/_utils/merger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_utils/net.py` & `dagster-1.3.6/dagster/_utils/net.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_utils/schedules.py` & `dagster-1.3.6/dagster/_utils/schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_utils/tags.py` & `dagster-1.3.6/dagster/_utils/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_utils/temp_file.py` & `dagster-1.3.6/dagster/_utils/temp_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_utils/test/__init__.py` & `dagster-1.3.6/dagster/_utils/test/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_utils/test/mysql_instance.py` & `dagster-1.3.6/dagster/_utils/test/mysql_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_utils/test/postgres_instance.py` & `dagster-1.3.6/dagster/_utils/test/postgres_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_utils/test/schedule_storage.py` & `dagster-1.3.6/dagster/_utils/test/schedule_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import sys
 import time
 
 import pendulum
 import pytest
 
+from dagster import StaticPartitionsDefinition
 from dagster._core.definitions.asset_reconciliation_sensor import (
     AutoMaterializeAssetEvaluation,
 )
 from dagster._core.definitions.auto_materialize_condition import MissingAutoMaterializeCondition
 from dagster._core.definitions.events import AssetKey
+from dagster._core.definitions.partition import SerializedPartitionsSubset
 from dagster._core.host_representation import (
     ExternalRepositoryOrigin,
     ManagedGrpcPythonEnvCodeLocationOrigin,
 )
 from dagster._core.scheduler.instigation import (
     InstigatorState,
     InstigatorStatus,
@@ -683,22 +685,22 @@
             pytest.skip("Storage cannot store auto materialize asset evaluations")
 
         storage.add_auto_materialize_asset_evaluations(
             evaluation_id=10,
             asset_evaluations=[
                 AutoMaterializeAssetEvaluation(
                     asset_key=AssetKey("asset_one"),
-                    conditions=[],
+                    partition_subsets_by_condition=[],
                     num_requested=0,
                     num_skipped=0,
                     num_discarded=0,
                 ),
                 AutoMaterializeAssetEvaluation(
                     asset_key=AssetKey("asset_two"),
-                    conditions=[MissingAutoMaterializeCondition()],
+                    partition_subsets_by_condition=[(MissingAutoMaterializeCondition(), None)],
                     num_requested=1,
                     num_skipped=0,
                     num_discarded=0,
                 ),
             ],
         )
 
@@ -719,15 +721,15 @@
         assert res[0].evaluation.num_requested == 1
 
         storage.add_auto_materialize_asset_evaluations(
             evaluation_id=11,
             asset_evaluations=[
                 AutoMaterializeAssetEvaluation(
                     asset_key=AssetKey("asset_one"),
-                    conditions=[],
+                    partition_subsets_by_condition=[],
                     num_requested=0,
                     num_skipped=0,
                     num_discarded=0,
                 ),
             ],
         )
 
@@ -745,7 +747,54 @@
         assert res[0].evaluation_id == 11
 
         res = storage.get_auto_materialize_asset_evaluations(
             asset_key=AssetKey("asset_one"), limit=1, cursor=11
         )
         assert len(res) == 1
         assert res[0].evaluation_id == 10
+
+    def test_auto_materialize_asset_evaluations_with_partitions(self, storage):
+        if not self.can_store_auto_materialize_asset_evaluations():
+            pytest.skip("Storage cannot store auto materialize asset evaluations")
+
+        partitions_def = StaticPartitionsDefinition(["a", "b"])
+        subset = partitions_def.empty_subset().with_partition_keys(["a"])
+
+        storage.add_auto_materialize_asset_evaluations(
+            evaluation_id=10,
+            asset_evaluations=[
+                AutoMaterializeAssetEvaluation(
+                    asset_key=AssetKey("asset_two"),
+                    partition_subsets_by_condition=[
+                        (
+                            MissingAutoMaterializeCondition(),
+                            SerializedPartitionsSubset.from_subset(subset, partitions_def, None),
+                        )
+                    ],
+                    num_requested=1,
+                    num_skipped=0,
+                    num_discarded=0,
+                ),
+            ],
+        )
+
+        res = storage.get_auto_materialize_asset_evaluations(
+            asset_key=AssetKey("asset_two"), limit=100
+        )
+        assert len(res) == 1
+        assert res[0].evaluation.asset_key == AssetKey("asset_two")
+        assert res[0].evaluation_id == 10
+        assert res[0].evaluation.num_requested == 1
+
+        assert (
+            res[0].evaluation.partition_subsets_by_condition[0][0]
+            == MissingAutoMaterializeCondition()
+        )
+        assert (
+            res[0].evaluation.partition_subsets_by_condition[0][1].can_deserialize(partitions_def)
+        )
+        assert (
+            partitions_def.deserialize_subset(
+                res[0].evaluation.partition_subsets_by_condition[0][1].serialized_subset
+            )
+            == subset
+        )
```

### Comparing `dagster-1.3.5/dagster/_utils/timing.py` & `dagster-1.3.6/dagster/_utils/timing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_utils/typing_api.py` & `dagster-1.3.6/dagster/_utils/typing_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster/_utils/yaml_utils.py` & `dagster-1.3.6/dagster/_utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.5/dagster.egg-info/PKG-INFO` & `dagster-1.3.6/dagster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.3.5
+Version: 1.3.6
 Summary: The data orchestration platform built for productivity.
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Changelog, https://github.com/dagster-io/dagster/releases
```

### Comparing `dagster-1.3.5/dagster.egg-info/SOURCES.txt` & `dagster-1.3.6/dagster.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 dagster/_api/snapshot_schedule.py
 dagster/_api/snapshot_sensor.py
 dagster/_check/README.md
 dagster/_check/__init__.py
 dagster/_cli/__init__.py
 dagster/_cli/api.py
 dagster/_cli/asset.py
+dagster/_cli/code_server.py
 dagster/_cli/config_scaffolder.py
 dagster/_cli/debug.py
 dagster/_cli/dev.py
 dagster/_cli/instance.py
 dagster/_cli/job.py
 dagster/_cli/load_handle.py
 dagster/_cli/project.py
@@ -486,14 +487,15 @@
 dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
 dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
 dagster/_grpc/__init__.py
 dagster/_grpc/__main__.py
 dagster/_grpc/client.py
 dagster/_grpc/compile.py
 dagster/_grpc/impl.py
+dagster/_grpc/proxy_server.py
 dagster/_grpc/server.py
 dagster/_grpc/server_watcher.py
 dagster/_grpc/types.py
 dagster/_grpc/utils.py
 dagster/_grpc/__generated__/__init__.py
 dagster/_grpc/__generated__/api_pb2.py
 dagster/_grpc/__generated__/api_pb2_grpc.py
```

### Comparing `dagster-1.3.5/dagster.egg-info/requires.txt` & `dagster-1.3.6/dagster.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 tqdm
 typing_extensions>=4.4.0
 sqlalchemy<2.0.0,>=1.0
 toposort>=1.0
 watchdog>=0.8.3
 docstring-parser
 universal_pathlib
-pydantic
+pydantic!=1.10.7
 
 [:platform_system == "Windows"]
 psutil>=1.0
 pywin32!=226
 
 [:python_version < "3.11"]
 grpcio<1.48.0,>=1.44.0
```

### Comparing `dagster-1.3.5/setup.py` & `dagster-1.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,16 @@
         "toposort>=1.0",
         "watchdog>=0.8.3",
         'psutil >= 1.0; platform_system=="Windows"',
         # https://github.com/mhammond/pywin32/issues/1439
         'pywin32 != 226; platform_system=="Windows"',
         "docstring-parser",
         "universal_pathlib",
-        "pydantic",
+        # https://github.com/pydantic/pydantic/issues/5821
+        "pydantic != 1.10.7",
     ],
     extras_require={
         "docker": ["docker"],
         "test": [
             "buildkite-test-collector ; python_version>='3.8'",
             "docker",
             "grpcio-tools>=1.44.0",  # related to above grpcio pins
```

