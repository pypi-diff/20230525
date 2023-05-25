# Comparing `tmp/dagster-graphql-1.3.5.tar.gz` & `tmp/dagster-graphql-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-graphql-1.3.5.tar", last modified: Thu May 18 20:45:04 2023, max compression
+gzip compressed data, was "dagster-graphql-1.3.6.tar", last modified: Thu May 25 17:23:41 2023, max compression
```

## Comparing `dagster-graphql-1.3.5.tar` & `dagster-graphql-1.3.6.tar`

### file list

```diff
@@ -1,117 +1,119 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:45:04.129603 dagster-graphql-1.3.5/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      654 2023-05-18 20:45:04.129603 dagster-graphql-1.3.5/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:45:04.009603 dagster-graphql-1.3.5/dagster_graphql/
--rw-r--r--   0 root         (0) root         (0)      641 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7374 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:45:04.013603 dagster-graphql-1.3.5/dagster_graphql/client/
--rw-r--r--   0 root         (0) root         (0)      482 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17835 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/client/client.py
--rw-r--r--   0 root         (0) root         (0)     2715 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/client/client_queries.py
--rw-r--r--   0 root         (0) root         (0)     6886 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/client/query.py
--rw-r--r--   0 root         (0) root         (0)     2917 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/client/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:45:04.029603 dagster-graphql-1.3.5/dagster_graphql/implementation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18592 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:45:04.033603 dagster-graphql-1.3.5/dagster_graphql/implementation/execution/
--rw-r--r--   0 root         (0) root         (0)    11457 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8885 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     3725 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/execution/dynamic_partitions.py
--rw-r--r--   0 root         (0) root         (0)     4586 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/execution/launch_execution.py
--rw-r--r--   0 root         (0) root         (0)     4396 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/execution/run_lifecycle.py
--rw-r--r--   0 root         (0) root         (0)     7270 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/external.py
--rw-r--r--   0 root         (0) root         (0)    25629 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_assets.py
--rw-r--r--   0 root         (0) root         (0)     1237 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_backfills.py
--rw-r--r--   0 root         (0) root         (0)     1120 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_env_vars.py
--rw-r--r--   0 root         (0) root         (0)     4346 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_instigators.py
--rw-r--r--   0 root         (0) root         (0)      951 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_logs.py
--rw-r--r--   0 root         (0) root         (0)    12470 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_partition_sets.py
--rw-r--r--   0 root         (0) root         (0)     3726 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     2431 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_resources.py
--rw-r--r--   0 root         (0) root         (0)    14972 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_runs.py
--rw-r--r--   0 root         (0) root         (0)     8157 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_schedules.py
--rw-r--r--   0 root         (0) root         (0)     9554 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_sensors.py
--rw-r--r--   0 root         (0) root         (0)     2910 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_solids.py
--rw-r--r--   0 root         (0) root         (0)    21120 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/loader.py
--rw-r--r--   0 root         (0) root         (0)     3093 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)      933 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     8078 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/implementation/utils.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:45:04.065603 dagster-graphql-1.3.5/dagster_graphql/schema/
--rw-r--r--   0 root         (0) root         (0)     2907 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40498 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)      385 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/asset_key.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/auto_materialize_policy.py
--rw-r--r--   0 root         (0) root         (0)    16767 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/backfill.py
--rw-r--r--   0 root         (0) root         (0)      627 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/config_type_or_error.py
--rw-r--r--   0 root         (0) root         (0)    15855 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/config_types.py
--rw-r--r--   0 root         (0) root         (0)     4785 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/env_vars.py
--rw-r--r--   0 root         (0) root         (0)    18061 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/errors.py
--rw-r--r--   0 root         (0) root         (0)     5489 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/execution.py
--rw-r--r--   0 root         (0) root         (0)    16323 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/external.py
--rw-r--r--   0 root         (0) root         (0)     1020 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    10983 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/inputs.py
--rw-r--r--   0 root         (0) root         (0)     5072 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/instance.py
--rw-r--r--   0 root         (0) root         (0)    28430 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/instigation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:45:04.069603 dagster-graphql-1.3.5/dagster_graphql/schema/logs/
--rw-r--r--   0 root         (0) root         (0)     3632 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2868 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/logs/compute_logs.py
--rw-r--r--   0 root         (0) root         (0)    20983 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/logs/events.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/logs/log_level.py
--rw-r--r--   0 root         (0) root         (0)     4473 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/metadata.py
--rw-r--r--   0 root         (0) root         (0)      111 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/paging.py
--rw-r--r--   0 root         (0) root         (0)    17622 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/partition_sets.py
--rw-r--r--   0 root         (0) root         (0)      748 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/permissions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:45:04.117603 dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/
--rw-r--r--   0 root         (0) root         (0)     3263 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11062 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/config.py
--rw-r--r--   0 root         (0) root         (0)      582 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/config_result.py
--rw-r--r--   0 root         (0) root         (0)     1369 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/logger.py
--rw-r--r--   0 root         (0) root         (0)     1826 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/mode.py
--rw-r--r--   0 root         (0) root         (0)    39385 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/pipeline.py
--rw-r--r--   0 root         (0) root         (0)      855 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/pipeline_ref.py
--rw-r--r--   0 root         (0) root         (0)     2213 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/pipeline_run_stats.py
--rw-r--r--   0 root         (0) root         (0)     1496 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/resource.py
--rw-r--r--   0 root         (0) root         (0)     1261 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/snapshot.py
--rw-r--r--   0 root         (0) root         (0)     1621 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/status.py
--rw-r--r--   0 root         (0) root         (0)      993 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/subscription.py
--rw-r--r--   0 root         (0) root         (0)     1658 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/repository_origin.py
--rw-r--r--   0 root         (0) root         (0)     8315 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:45:04.125603 dagster-graphql-1.3.5/dagster_graphql/schema/roots/
--rw-r--r--   0 root         (0) root         (0)     2094 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/roots/__init__.py
--rw-r--r--   0 root         (0) root         (0)      620 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/roots/assets.py
--rw-r--r--   0 root         (0) root         (0)      564 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/roots/execution_plan.py
--rw-r--r--   0 root         (0) root         (0)    25294 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/roots/mutation.py
--rw-r--r--   0 root         (0) root         (0)      723 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/roots/pipeline.py
--rw-r--r--   0 root         (0) root         (0)    36755 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/roots/query.py
--rw-r--r--   0 root         (0) root         (0)     2915 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/roots/subscription.py
--rw-r--r--   0 root         (0) root         (0)     5050 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/run_config.py
--rw-r--r--   0 root         (0) root         (0)     5940 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/runs.py
--rw-r--r--   0 root         (0) root         (0)     1438 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/schedule_dry_run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:45:04.129603 dagster-graphql-1.3.5/dagster_graphql/schema/schedules/
--rw-r--r--   0 root         (0) root         (0)     3904 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8306 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/schedules/schedules.py
--rw-r--r--   0 root         (0) root         (0)     1833 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/schedules/ticks.py
--rw-r--r--   0 root         (0) root         (0)     1312 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/sensor_dry_run.py
--rw-r--r--   0 root         (0) root         (0)     7983 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/sensors.py
--rw-r--r--   0 root         (0) root         (0)    29569 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/solids.py
--rw-r--r--   0 root         (0) root         (0)     1328 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/table.py
--rw-r--r--   0 root         (0) root         (0)     1411 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/tags.py
--rw-r--r--   0 root         (0) root         (0)      234 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/test.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/used_solid.py
--rw-r--r--   0 root         (0) root         (0)      950 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/schema/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:45:04.129603 dagster-graphql-1.3.5/dagster_graphql/test/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6364 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/test/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/dagster_graphql/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:45:04.009603 dagster-graphql-1.3.5/dagster_graphql.egg-info/
--rw-r--r--   0 root         (0) root         (0)      654 2023-05-18 20:45:03.000000 dagster-graphql-1.3.5/dagster_graphql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4150 2023-05-18 20:45:03.000000 dagster-graphql-1.3.5/dagster_graphql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 20:45:03.000000 dagster-graphql-1.3.5/dagster_graphql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-05-18 20:45:03.000000 dagster-graphql-1.3.5/dagster_graphql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       81 2023-05-18 20:45:03.000000 dagster-graphql-1.3.5/dagster_graphql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-18 20:45:03.000000 dagster-graphql-1.3.5/dagster_graphql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      180 2023-05-18 20:45:04.133603 dagster-graphql-1.3.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1527 2023-05-18 20:38:07.000000 dagster-graphql-1.3.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:23:41.969202 dagster-graphql-1.3.6/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      654 2023-05-25 17:23:41.969202 dagster-graphql-1.3.6/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:23:41.885201 dagster-graphql-1.3.6/dagster_graphql/
+-rw-r--r--   0 root         (0) root         (0)      641 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7442 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:23:41.889201 dagster-graphql-1.3.6/dagster_graphql/client/
+-rw-r--r--   0 root         (0) root         (0)      482 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17835 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     2715 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/client/client_queries.py
+-rw-r--r--   0 root         (0) root         (0)     6886 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/client/query.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/client/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:23:41.905202 dagster-graphql-1.3.6/dagster_graphql/implementation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18592 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:23:41.909201 dagster-graphql-1.3.6/dagster_graphql/implementation/execution/
+-rw-r--r--   0 root         (0) root         (0)    11457 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8885 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     3725 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/execution/dynamic_partitions.py
+-rw-r--r--   0 root         (0) root         (0)     4586 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/execution/launch_execution.py
+-rw-r--r--   0 root         (0) root         (0)     4396 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/execution/run_lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)     7270 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/external.py
+-rw-r--r--   0 root         (0) root         (0)    25777 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_assets.py
+-rw-r--r--   0 root         (0) root         (0)     1330 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)     1237 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_backfills.py
+-rw-r--r--   0 root         (0) root         (0)     1120 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_env_vars.py
+-rw-r--r--   0 root         (0) root         (0)     4346 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_instigators.py
+-rw-r--r--   0 root         (0) root         (0)      951 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_logs.py
+-rw-r--r--   0 root         (0) root         (0)    12470 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)     3726 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     2431 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_resources.py
+-rw-r--r--   0 root         (0) root         (0)    14972 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_runs.py
+-rw-r--r--   0 root         (0) root         (0)     8157 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_schedules.py
+-rw-r--r--   0 root         (0) root         (0)     9554 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_sensors.py
+-rw-r--r--   0 root         (0) root         (0)     2910 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_solids.py
+-rw-r--r--   0 root         (0) root         (0)    21120 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/loader.py
+-rw-r--r--   0 root         (0) root         (0)     3093 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)      933 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     8078 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/implementation/utils.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:23:41.937202 dagster-graphql-1.3.6/dagster_graphql/schema/
+-rw-r--r--   0 root         (0) root         (0)     2907 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40571 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)      385 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/asset_key.py
+-rw-r--r--   0 root         (0) root         (0)     4705 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/auto_materialize_asset_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16767 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/backfill.py
+-rw-r--r--   0 root         (0) root         (0)      627 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/config_type_or_error.py
+-rw-r--r--   0 root         (0) root         (0)    15855 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     4785 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/env_vars.py
+-rw-r--r--   0 root         (0) root         (0)    18061 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/errors.py
+-rw-r--r--   0 root         (0) root         (0)     5489 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/execution.py
+-rw-r--r--   0 root         (0) root         (0)    16323 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/external.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    10983 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     5072 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/instance.py
+-rw-r--r--   0 root         (0) root         (0)    28430 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/instigation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:23:41.941202 dagster-graphql-1.3.6/dagster_graphql/schema/logs/
+-rw-r--r--   0 root         (0) root         (0)     3632 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2868 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/logs/compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)    20983 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/logs/events.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/logs/log_level.py
+-rw-r--r--   0 root         (0) root         (0)     4473 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/metadata.py
+-rw-r--r--   0 root         (0) root         (0)      111 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/paging.py
+-rw-r--r--   0 root         (0) root         (0)    17622 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)      748 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/permissions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:23:41.957202 dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/
+-rw-r--r--   0 root         (0) root         (0)     3263 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11062 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/config.py
+-rw-r--r--   0 root         (0) root         (0)      582 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/config_result.py
+-rw-r--r--   0 root         (0) root         (0)     1369 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1826 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/mode.py
+-rw-r--r--   0 root         (0) root         (0)    39668 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)      855 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/pipeline_ref.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/pipeline_run_stats.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1261 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/status.py
+-rw-r--r--   0 root         (0) root         (0)      993 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/repository_origin.py
+-rw-r--r--   0 root         (0) root         (0)     8315 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:23:41.965202 dagster-graphql-1.3.6/dagster_graphql/schema/roots/
+-rw-r--r--   0 root         (0) root         (0)     2094 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/roots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      620 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/roots/assets.py
+-rw-r--r--   0 root         (0) root         (0)      564 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/roots/execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)    25389 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/roots/mutation.py
+-rw-r--r--   0 root         (0) root         (0)      723 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/roots/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    37776 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/roots/query.py
+-rw-r--r--   0 root         (0) root         (0)     2915 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/roots/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     5050 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     5940 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/runs.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/schedule_dry_run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:23:41.965202 dagster-graphql-1.3.6/dagster_graphql/schema/schedules/
+-rw-r--r--   0 root         (0) root         (0)     3904 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8306 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/schedules/schedules.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/schedules/ticks.py
+-rw-r--r--   0 root         (0) root         (0)     1312 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/sensor_dry_run.py
+-rw-r--r--   0 root         (0) root         (0)     7983 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/sensors.py
+-rw-r--r--   0 root         (0) root         (0)    29569 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/solids.py
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/table.py
+-rw-r--r--   0 root         (0) root         (0)     1411 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/tags.py
+-rw-r--r--   0 root         (0) root         (0)      234 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/test.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/used_solid.py
+-rw-r--r--   0 root         (0) root         (0)      950 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/schema/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:23:41.965202 dagster-graphql-1.3.6/dagster_graphql/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6364 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/test/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/dagster_graphql/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:23:41.889201 dagster-graphql-1.3.6/dagster_graphql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      654 2023-05-25 17:23:41.000000 dagster-graphql-1.3.6/dagster_graphql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4286 2023-05-25 17:23:41.000000 dagster-graphql-1.3.6/dagster_graphql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 17:23:41.000000 dagster-graphql-1.3.6/dagster_graphql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-05-25 17:23:41.000000 dagster-graphql-1.3.6/dagster_graphql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       81 2023-05-25 17:23:41.000000 dagster-graphql-1.3.6/dagster_graphql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-25 17:23:41.000000 dagster-graphql-1.3.6/dagster_graphql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      180 2023-05-25 17:23:41.969202 dagster-graphql-1.3.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-05-25 17:16:49.000000 dagster-graphql-1.3.6/setup.py
```

### Comparing `dagster-graphql-1.3.5/LICENSE` & `dagster-graphql-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/PKG-INFO` & `dagster-graphql-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.3.5
+Version: 1.3.6
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-graphql-1.3.5/dagster_graphql/__init__.py` & `dagster-graphql-1.3.6/dagster_graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/cli.py` & `dagster-graphql-1.3.6/dagster_graphql/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,24 +192,26 @@
             "to select GraphQL document to execute."
         )
 
     if remote:
         res = execute_query_against_remote(remote, query, variables)
         print(res)  # noqa: T201
     else:
-        instance = DagsterInstance.ephemeral() if ephemeral_instance else DagsterInstance.get()
-        with get_workspace_process_context_from_kwargs(
-            instance, version=__version__, read_only=False, kwargs=kwargs
-        ) as workspace_process_context:
-            execute_query_from_cli(
-                workspace_process_context,
-                query,
-                variables,
-                output,
-            )
+        with (
+            DagsterInstance.local_temp() if ephemeral_instance else DagsterInstance.get()
+        ) as instance:
+            with get_workspace_process_context_from_kwargs(
+                instance, version=__version__, read_only=False, kwargs=kwargs
+            ) as workspace_process_context:
+                execute_query_from_cli(
+                    workspace_process_context,
+                    query,
+                    variables,
+                    output,
+                )
 
 
 cli = create_dagster_graphql_cli()
 
 
 def main():
     # click magic
```

### Comparing `dagster-graphql-1.3.5/dagster_graphql/client/client.py` & `dagster-graphql-1.3.6/dagster_graphql/client/client.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/client/client_queries.py` & `dagster-graphql-1.3.6/dagster_graphql/client/client_queries.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/client/query.py` & `dagster-graphql-1.3.6/dagster_graphql/client/query.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/client/utils.py` & `dagster-graphql-1.3.6/dagster_graphql/client/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/implementation/events.py` & `dagster-graphql-1.3.6/dagster_graphql/implementation/events.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/implementation/execution/__init__.py` & `dagster-graphql-1.3.6/dagster_graphql/implementation/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/implementation/execution/backfill.py` & `dagster-graphql-1.3.6/dagster_graphql/implementation/execution/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/implementation/execution/dynamic_partitions.py` & `dagster-graphql-1.3.6/dagster_graphql/implementation/execution/dynamic_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/implementation/execution/launch_execution.py` & `dagster-graphql-1.3.6/dagster_graphql/implementation/execution/launch_execution.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/implementation/execution/run_lifecycle.py` & `dagster-graphql-1.3.6/dagster_graphql/implementation/execution/run_lifecycle.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/implementation/external.py` & `dagster-graphql-1.3.6/dagster_graphql/implementation/external.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_assets.py` & `dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_assets.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,17 +62,17 @@
 
 if TYPE_CHECKING:
     from ..schema.asset_graph import GrapheneAssetNode, GrapheneAssetNodeDefinitionCollision
     from ..schema.errors import GrapheneAssetNotFoundError
     from ..schema.freshness_policy import GrapheneAssetFreshnessInfo
     from ..schema.pipelines.pipeline import (
         GrapheneAsset,
-        GrapheneDefaultPartitions,
-        GrapheneMultiPartitions,
-        GrapheneTimePartitions,
+        GrapheneDefaultPartitionStatuses,
+        GrapheneMultiPartitionStatuses,
+        GrapheneTimePartitionStatuses,
     )
     from ..schema.roots.assets import GrapheneAssetConnection
     from ..schema.util import ResolveInfo
 
 
 def _normalize_asset_cursor_str(cursor_string: Optional[str]) -> Optional[str]:
     # the cursor for assets is derived from a json serialized string of the path.  Because there are
@@ -401,27 +401,31 @@
 
 
 def build_partition_statuses(
     dynamic_partitions_store: DynamicPartitionsStore,
     materialized_partitions_subset: Optional[PartitionsSubset],
     failed_partitions_subset: Optional[PartitionsSubset],
     in_progress_partitions_subset: Optional[PartitionsSubset],
-) -> Union["GrapheneTimePartitions", "GrapheneDefaultPartitions", "GrapheneMultiPartitions"]:
+) -> Union[
+    "GrapheneTimePartitionStatuses",
+    "GrapheneDefaultPartitionStatuses",
+    "GrapheneMultiPartitionStatuses",
+]:
     from ..schema.pipelines.pipeline import (
-        GrapheneDefaultPartitions,
-        GrapheneTimePartitionRange,
-        GrapheneTimePartitions,
+        GrapheneDefaultPartitionStatuses,
+        GrapheneTimePartitionRangeStatus,
+        GrapheneTimePartitionStatuses,
     )
 
     if (
         materialized_partitions_subset is None
         and failed_partitions_subset is None
         and in_progress_partitions_subset is None
     ):
-        return GrapheneDefaultPartitions(
+        return GrapheneDefaultPartitionStatuses(
             materializedPartitions=[],
             failedPartitions=[],
             unmaterializedPartitions=[],
             materializingPartitions=[],
         )
 
     materialized_partitions_subset = check.not_none(materialized_partitions_subset)
@@ -451,36 +455,36 @@
         )
         graphene_ranges = []
         for r in ranges:
             partition_key_range = cast(
                 TimeWindowPartitionsDefinition, materialized_partitions_subset.partitions_def
             ).get_partition_key_range_for_time_window(r.time_window)
             graphene_ranges.append(
-                GrapheneTimePartitionRange(
+                GrapheneTimePartitionRangeStatus(
                     startTime=r.time_window.start.timestamp(),
                     endTime=r.time_window.end.timestamp(),
                     startKey=partition_key_range.start,
                     endKey=partition_key_range.end,
                     status=r.status,
                 )
             )
-        return GrapheneTimePartitions(ranges=graphene_ranges)
+        return GrapheneTimePartitionStatuses(ranges=graphene_ranges)
     elif isinstance(materialized_partitions_subset, MultiPartitionsSubset):
         return get_2d_run_length_encoded_partitions(
             dynamic_partitions_store,
             materialized_partitions_subset,
             failed_partitions_subset,
             in_progress_partitions_subset,
         )
     elif isinstance(materialized_partitions_subset, DefaultPartitionsSubset):
         materialized_keys = materialized_partitions_subset.get_partition_keys()
         failed_keys = failed_partitions_subset.get_partition_keys()
         in_progress_keys = in_progress_partitions_subset.get_partition_keys()
 
-        return GrapheneDefaultPartitions(
+        return GrapheneDefaultPartitionStatuses(
             materializedPartitions=set(materialized_keys)
             - set(failed_keys)
             - set(in_progress_keys),
             failedPartitions=failed_keys,
             unmaterializedPartitions=materialized_partitions_subset.get_partition_keys_not_in_subset(
                 dynamic_partitions_store=dynamic_partitions_store
             ),
@@ -491,18 +495,18 @@
 
 
 def get_2d_run_length_encoded_partitions(
     dynamic_partitions_store: DynamicPartitionsStore,
     materialized_partitions_subset: PartitionsSubset,
     failed_partitions_subset: PartitionsSubset,
     in_progress_partitions_subset: PartitionsSubset,
-) -> "GrapheneMultiPartitions":
+) -> "GrapheneMultiPartitionStatuses":
     from ..schema.pipelines.pipeline import (
-        GrapheneMultiPartitionRange,
-        GrapheneMultiPartitions,
+        GrapheneMultiPartitionRangeStatuses,
+        GrapheneMultiPartitionStatuses,
     )
 
     if (
         not isinstance(materialized_partitions_subset.partitions_def, MultiPartitionsDefinition)
         or not isinstance(failed_partitions_subset.partitions_def, MultiPartitionsDefinition)
         or not isinstance(in_progress_partitions_subset.partitions_def, MultiPartitionsDefinition)
     ):
@@ -566,15 +570,15 @@
         or len(
             secondary_dim.partitions_def.get_partition_keys(
                 dynamic_partitions_store=dynamic_partitions_store
             )
         )
         == 0
     ):
-        return GrapheneMultiPartitions(ranges=[], primaryDimensionName=primary_dim.name)
+        return GrapheneMultiPartitionStatuses(ranges=[], primaryDimensionName=primary_dim.name)
 
     while unevaluated_idx <= len(dim1_keys):
         if (
             unevaluated_idx == len(dim1_keys)
             or dim2_materialized_partition_subset_by_dim1[dim1_keys[unevaluated_idx]]
             != dim2_materialized_partition_subset_by_dim1[dim1_keys[range_start_idx]]
             or dim2_failed_partition_subset_by_dim1[dim1_keys[unevaluated_idx]]
@@ -601,15 +605,15 @@
                     start_time = time_windows[0].start.timestamp()
                     end_time = time_windows[-1].end.timestamp()
                 else:
                     start_time = None
                     end_time = None
 
                 materialized_2d_ranges.append(
-                    GrapheneMultiPartitionRange(
+                    GrapheneMultiPartitionRangeStatuses(
                         primaryDimStartKey=start_key,
                         primaryDimEndKey=end_key,
                         primaryDimStartTime=start_time,
                         primaryDimEndTime=end_time,
                         secondaryDim=build_partition_statuses(
                             dynamic_partitions_store,
                             dim2_materialized_partition_subset_by_dim1[start_key],
@@ -617,15 +621,15 @@
                             dim2_in_progress_partition_subset_by_dim1[start_key],
                         ),
                     )
                 )
             range_start_idx = unevaluated_idx
         unevaluated_idx += 1
 
-    return GrapheneMultiPartitions(
+    return GrapheneMultiPartitionStatuses(
         ranges=materialized_2d_ranges, primaryDimensionName=primary_dim.name
     )
 
 
 def get_freshness_info(
     asset_key: AssetKey,
     data_time_resolver: CachingDataTimeResolver,
```

### Comparing `dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_backfills.py` & `dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_backfills.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_env_vars.py` & `dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_env_vars.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_instigators.py` & `dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_instigators.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_logs.py` & `dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_partition_sets.py` & `dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_partition_sets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_pipelines.py` & `dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_pipelines.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_resources.py` & `dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_runs.py` & `dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_runs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_schedules.py` & `dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_sensors.py` & `dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/implementation/fetch_solids.py` & `dagster-graphql-1.3.6/dagster_graphql/implementation/fetch_solids.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/implementation/loader.py` & `dagster-graphql-1.3.6/dagster_graphql/implementation/loader.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/implementation/run_config_schema.py` & `dagster-graphql-1.3.6/dagster_graphql/implementation/run_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/implementation/telemetry.py` & `dagster-graphql-1.3.6/dagster_graphql/implementation/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/implementation/utils.py` & `dagster-graphql-1.3.6/dagster_graphql/implementation/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/__init__.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/asset_graph.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/asset_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,20 +69,20 @@
     to_dagster_type,
 )
 from .errors import GrapheneAssetNotFoundError
 from .freshness_policy import GrapheneAssetFreshnessInfo, GrapheneFreshnessPolicy
 from .logs.events import GrapheneMaterializationEvent, GrapheneObservationEvent
 from .pipelines.pipeline import (
     GrapheneAssetPartitionStatuses,
-    GrapheneDefaultPartitions,
-    GrapheneMultiPartitions,
+    GrapheneDefaultPartitionStatuses,
+    GrapheneMultiPartitionStatuses,
     GraphenePartitionStats,
     GraphenePipeline,
     GrapheneRun,
-    GrapheneTimePartitions,
+    GrapheneTimePartitionStatuses,
 )
 from .util import ResolveInfo, non_null_list
 
 if TYPE_CHECKING:
     from .external import GrapheneRepository
 
 GrapheneAssetStaleStatus = graphene.Enum.from_enum(StaleStatus, name="StaleStatus")
@@ -786,15 +786,19 @@
         if not event_records:
             return None
         run_record = graphene_info.context.instance.get_run_record_by_id(event_records[0].run_id)
         return GrapheneRun(run_record) if run_record else None
 
     def resolve_assetPartitionStatuses(
         self, graphene_info: ResolveInfo
-    ) -> Union["GrapheneTimePartitions", "GrapheneDefaultPartitions", "GrapheneMultiPartitions"]:
+    ) -> Union[
+        "GrapheneTimePartitionStatuses",
+        "GrapheneDefaultPartitionStatuses",
+        "GrapheneMultiPartitionStatuses",
+    ]:
         asset_key = self._external_asset_node.asset_key
 
         if not self._dynamic_partitions_loader:
             check.failed("dynamic_partitions_loader must be provided to get partition keys")
 
         (
             materialized_partition_subset,
```

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/auto_materialize_policy.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/auto_materialize_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/backfill.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/config_type_or_error.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/config_type_or_error.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/config_types.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/config_types.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/dagster_types.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/env_vars.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/env_vars.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/errors.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/execution.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/external.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/external.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/freshness_policy.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/inputs.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/inputs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/instance.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/instance.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/instigation.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/instigation.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/logs/__init__.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/logs/compute_logs.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/logs/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/logs/events.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/logs/events.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/logs/log_level.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/logs/log_level.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/metadata.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/metadata.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/partition_sets.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/partition_sets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/permissions.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/__init__.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/config.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/config.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/config_result.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/config_result.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/logger.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/mode.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/pipeline.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,74 +85,84 @@
         return None
 
 
 GraphenePartitionRangeStatus = graphene.Enum.from_enum(PartitionRangeStatus)
 
 
 class GrapheneTimePartitionRange(graphene.ObjectType):
-    status = graphene.NonNull(GraphenePartitionRangeStatus)
     startTime = graphene.NonNull(graphene.Float)
     endTime = graphene.NonNull(graphene.Float)
     startKey = graphene.NonNull(graphene.String)
     endKey = graphene.NonNull(graphene.String)
 
     class Meta:
         name = "TimePartitionRange"
 
 
-class GrapheneTimePartitions(graphene.ObjectType):
-    ranges = non_null_list(GrapheneTimePartitionRange)
+class GrapheneTimePartitionRangeStatus(GrapheneTimePartitionRange):
+    status = graphene.NonNull(GraphenePartitionRangeStatus)
+
+    class Meta:
+        name = "TimePartitionRangeStatus"
+
+
+class GrapheneTimePartitionStatuses(graphene.ObjectType):
+    ranges = non_null_list(GrapheneTimePartitionRangeStatus)
 
     class Meta:
-        name = "TimePartitions"
+        name = "TimePartitionStatuses"
 
 
-class GrapheneDefaultPartitions(graphene.ObjectType):
+class GrapheneDefaultPartitionStatuses(graphene.ObjectType):
     materializedPartitions = non_null_list(graphene.String)
     failedPartitions = non_null_list(graphene.String)
     unmaterializedPartitions = non_null_list(graphene.String)
     materializingPartitions = non_null_list(graphene.String)
 
     class Meta:
-        name = "DefaultPartitions"
+        name = "DefaultPartitionStatuses"
 
 
 class GraphenePartitionStatus1D(graphene.Union):
     class Meta:
-        types = (GrapheneTimePartitions, GrapheneDefaultPartitions)
+        types = (GrapheneTimePartitionStatuses, GrapheneDefaultPartitionStatuses)
         name = "PartitionStatus1D"
 
 
-class GrapheneMultiPartitionRange(graphene.ObjectType):
+class GrapheneMultiPartitionRangeStatuses(graphene.ObjectType):
     """The primary dimension of a multipartitioned asset is the time-partitioned dimension.
     If both dimensions of the asset are static or time-partitioned, the primary dimension is
     the first defined dimension.
     """
 
     primaryDimStartKey = graphene.NonNull(graphene.String)
     primaryDimEndKey = graphene.NonNull(graphene.String)
     primaryDimStartTime = graphene.Field(graphene.Float)
     primaryDimEndTime = graphene.Field(graphene.Float)
     secondaryDim = graphene.NonNull(GraphenePartitionStatus1D)
 
     class Meta:
-        name = "MaterializedPartitionRange2D"
+        name = "MaterializedPartitionRangeStatuses2D"
 
 
-class GrapheneMultiPartitions(graphene.ObjectType):
-    ranges = non_null_list(GrapheneMultiPartitionRange)
+class GrapheneMultiPartitionStatuses(graphene.ObjectType):
+    ranges = non_null_list(GrapheneMultiPartitionRangeStatuses)
     primaryDimensionName = graphene.NonNull(graphene.String)
 
     class Meta:
-        name = "MultiPartitions"
+        name = "MultiPartitionStatuses"
 
 
 class GrapheneAssetPartitionStatuses(graphene.Union):
     class Meta:
-        types = (GrapheneDefaultPartitions, GrapheneMultiPartitions, GrapheneTimePartitions)
+        types = (
+            GrapheneDefaultPartitionStatuses,
+            GrapheneMultiPartitionStatuses,
+            GrapheneTimePartitionStatuses,
+        )
         name = "AssetPartitionStatuses"
 
 
 class GraphenePartitionStats(graphene.ObjectType):
     numMaterialized = graphene.NonNull(graphene.Int)
     numPartitions = graphene.NonNull(graphene.Int)
     numFailed = graphene.NonNull(graphene.Int)
```

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/pipeline_ref.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/pipeline_ref.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/pipeline_run_stats.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/pipeline_run_stats.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/resource.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/snapshot.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/status.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/status.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/pipelines/subscription.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/pipelines/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/repository_origin.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/repository_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/resources.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/roots/__init__.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/roots/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/roots/assets.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/roots/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/roots/execution_plan.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/roots/execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/roots/mutation.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/roots/mutation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Optional, Sequence, Union
 
 import dagster._check as check
 import graphene
 from dagster._core.definitions.events import AssetKey
+from dagster._core.errors import DagsterInvariantViolationError
 from dagster._core.nux import get_has_seen_nux, set_nux_seen
 from dagster._core.workspace.permissions import Permissions
 from dagster._daemon.asset_daemon import set_auto_materialize_paused
 
 from dagster_graphql.implementation.execution.backfill import (
     cancel_partition_backfill,
     create_and_launch_partition_backfill,
@@ -384,18 +385,18 @@
     @require_permission_check(Permissions.LAUNCH_PIPELINE_REEXECUTION)
     def mutate(
         self,
         graphene_info: ResolveInfo,
         executionParams: Optional[GrapheneExecutionParams] = None,
         reexecutionParams: Optional[GrapheneReexecutionParams] = None,
     ):
-        check.invariant(
-            bool(executionParams) != bool(reexecutionParams),
-            "Must only provide one of either executionParams or reexecutionParams",
-        )
+        if bool(executionParams) == bool(reexecutionParams):
+            raise DagsterInvariantViolationError(
+                "Must only provide one of either executionParams or reexecutionParams"
+            )
 
         if executionParams:
             return create_execution_params_and_launch_pipeline_reexec(
                 graphene_info,
                 execution_params_dict=executionParams,
             )
         elif reexecutionParams:
```

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/roots/pipeline.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/roots/pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/roots/query.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/roots/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,23 @@
     ScheduleSelector,
     SensorSelector,
 )
 from dagster._core.execution.backfill import BulkActionStatus
 from dagster._core.nux import get_has_seen_nux
 from dagster._core.scheduler.instigation import InstigatorStatus, InstigatorType
 
+from dagster_graphql.implementation.fetch_auto_materialize_asset_evaluations import (
+    fetch_auto_materialize_asset_evaluations,
+)
 from dagster_graphql.implementation.fetch_env_vars import get_utilized_env_vars_or_error
 from dagster_graphql.implementation.fetch_logs import get_captured_log_metadata
 from dagster_graphql.implementation.fetch_runs import get_assets_latest_info
+from dagster_graphql.schema.auto_materialize_asset_evaluations import (
+    GrapheneAutoMaterializeAssetEvaluationRecord,
+)
 from dagster_graphql.schema.env_vars import GrapheneEnvVarWithConsumersListOrError
 
 from ...implementation.external import (
     fetch_location_statuses,
     fetch_repositories,
     fetch_repository,
     fetch_workspace,
@@ -459,14 +465,22 @@
     )
 
     test = graphene.Field(
         GrapheneTestFields,
         description="Provides fields for testing behavior",
     )
 
+    autoMaterializeAssetEvaluations = graphene.Field(
+        non_null_list(GrapheneAutoMaterializeAssetEvaluationRecord),
+        assetKey=graphene.Argument(GrapheneAssetKeyInput),
+        limit=graphene.Argument(graphene.NonNull(graphene.Int)),
+        cursor=graphene.Argument(graphene.String),
+        description="Retrieve the auto materialization evaluation records for all assets.",
+    )
+
     @capture_error
     def resolve_repositoriesOrError(
         self,
         graphene_info: ResolveInfo,
         repositorySelector: Optional[GrapheneRepositorySelector] = None,
     ):
         if repositorySelector:
@@ -968,7 +982,18 @@
         return from_captured_log_data(log_data)
 
     def resolve_shouldShowNux(self, graphene_info):
         return graphene_info.context.instance.nux_enabled and not get_has_seen_nux()
 
     def resolve_test(self, _):
         return GrapheneTestFields()
+
+    def resolve_autoMaterializeAssetEvaluations(
+        self,
+        graphene_info: ResolveInfo,
+        assetKey: GrapheneAssetKeyInput,
+        limit: int,
+        cursor: Optional[str],
+    ):
+        return fetch_auto_materialize_asset_evaluations(
+            instance=graphene_info.context.instance, asset_key=assetKey, cursor=cursor, limit=limit
+        )
```

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/roots/subscription.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/roots/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/run_config.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/runs.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/runs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/schedule_dry_run.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/schedule_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/schedules/__init__.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/schedules/schedules.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/schedules/schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/schedules/ticks.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/schedules/ticks.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/sensor_dry_run.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/sensor_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/sensors.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/solids.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/solids.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/table.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/table.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/tags.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/used_solid.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/used_solid.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/schema/util.py` & `dagster-graphql-1.3.6/dagster_graphql/schema/util.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql/test/utils.py` & `dagster-graphql-1.3.6/dagster_graphql/test/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.5/dagster_graphql.egg-info/PKG-INFO` & `dagster-graphql-1.3.6/dagster_graphql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.3.5
+Version: 1.3.6
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-graphql-1.3.5/dagster_graphql.egg-info/SOURCES.txt` & `dagster-graphql-1.3.6/dagster_graphql.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 dagster_graphql/client/client_queries.py
 dagster_graphql/client/query.py
 dagster_graphql/client/utils.py
 dagster_graphql/implementation/__init__.py
 dagster_graphql/implementation/events.py
 dagster_graphql/implementation/external.py
 dagster_graphql/implementation/fetch_assets.py
+dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py
 dagster_graphql/implementation/fetch_backfills.py
 dagster_graphql/implementation/fetch_env_vars.py
 dagster_graphql/implementation/fetch_instigators.py
 dagster_graphql/implementation/fetch_logs.py
 dagster_graphql/implementation/fetch_partition_sets.py
 dagster_graphql/implementation/fetch_pipelines.py
 dagster_graphql/implementation/fetch_resources.py
@@ -40,14 +41,15 @@
 dagster_graphql/implementation/execution/backfill.py
 dagster_graphql/implementation/execution/dynamic_partitions.py
 dagster_graphql/implementation/execution/launch_execution.py
 dagster_graphql/implementation/execution/run_lifecycle.py
 dagster_graphql/schema/__init__.py
 dagster_graphql/schema/asset_graph.py
 dagster_graphql/schema/asset_key.py
+dagster_graphql/schema/auto_materialize_asset_evaluations.py
 dagster_graphql/schema/auto_materialize_policy.py
 dagster_graphql/schema/backfill.py
 dagster_graphql/schema/config_type_or_error.py
 dagster_graphql/schema/config_types.py
 dagster_graphql/schema/dagster_types.py
 dagster_graphql/schema/env_vars.py
 dagster_graphql/schema/errors.py
```

### Comparing `dagster-graphql-1.3.5/setup.py` & `dagster-graphql-1.3.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_graphql_tests*"]),
     install_requires=[
-        "dagster==1.3.5",
+        "dagster==1.3.6",
         "graphene>=3",
         "gql[requests]>=3.0.0",
         "requests",
         "starlette",  # used for run_in_threadpool utility fn
         "urllib3<2.0.0",  # https://github.com/psf/requests/issues/6432
     ],
     entry_points={"console_scripts": ["dagster-graphql = dagster_graphql.cli:main"]},
```

