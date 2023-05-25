# Comparing `tmp/codecarbon-2.2.1.tar.gz` & `tmp/codecarbon-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codecarbon-2.2.1.tar", last modified: Sat May 13 07:17:41 2023, max compression
+gzip compressed data, was "codecarbon-2.2.2.tar", last modified: Thu May 25 09:25:54 2023, max compression
```

## Comparing `codecarbon-2.2.1.tar` & `codecarbon-2.2.2.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:17:41.198661 codecarbon-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-13 07:17:25.000000 codecarbon-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-05-13 07:17:41.194661 codecarbon-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-05-13 07:17:25.000000 codecarbon-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:17:41.170661 codecarbon-2.2.1/carbonserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:17:25.000000 codecarbon-2.2.1/carbonserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:17:41.170661 codecarbon-2.2.1/carbonserver/carbonserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:17:25.000000 codecarbon-2.2.1/carbonserver/carbonserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:17:41.170661 codecarbon-2.2.1/carbonserver/carbonserver/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:17:25.000000 codecarbon-2.2.1/carbonserver/carbonserver/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-13 07:17:25.000000 codecarbon-2.2.1/carbonserver/carbonserver/api/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:17:41.174661 codecarbon-2.2.1/carbonserver/carbonserver/api/domain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:17:25.000000 codecarbon-2.2.1/carbonserver/carbonserver/api/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-13 07:17:25.000000 codecarbon-2.2.1/carbonserver/carbonserver/api/domain/emissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-13 07:17:25.000000 codecarbon-2.2.1/carbonserver/carbonserver/api/domain/experiments.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-13 07:17:25.000000 codecarbon-2.2.1/carbonserver/carbonserver/api/domain/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-13 07:17:25.000000 codecarbon-2.2.1/carbonserver/carbonserver/api/domain/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-13 07:17:25.000000 codecarbon-2.2.1/carbonserver/carbonserver/api/domain/runs.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-13 07:17:25.000000 codecarbon-2.2.1/carbonserver/carbonserver/api/domain/teams.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-13 07:17:25.000000 codecarbon-2.2.1/carbonserver/carbonserver/api/domain/users.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-13 07:17:25.000000 codecarbon-2.2.1/carbonserver/carbonserver/api/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:17:41.174661 codecarbon-2.2.1/carbonserver/carbonserver/api/routers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:17:25.000000 codecarbon-2.2.1/carbonserver/carbonserver/api/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-13 07:17:25.000000 codecarbon-2.2.1/carbonserver/carbonserver/api/routers/authenticate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-13 07:17:25.000000 codecarbon-2.2.1/carbonserver/carbonserver/api/routers/emissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-13 07:17:25.000000 codecarbon-2.2.1/carbonserver/carbonserver/api/routers/experiments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-13 07:17:25.000000 codecarbon-2.2.1/carbonserver/carbonserver/api/routers/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-13 07:17:25.000000 codecarbon-2.2.1/carbonserver/carbonserver/api/routers/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-05-13 07:17:25.000000 codecarbon-2.2.1/carbonserver/carbonserver/api/routers/runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-13 07:17:25.000000 codecarbon-2.2.1/carbonserver/carbonserver/api/routers/teams.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-13 07:17:25.000000 codecarbon-2.2.1/carbonserver/carbonserver/api/routers/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-05-13 07:17:25.000000 codecarbon-2.2.1/carbonserver/carbonserver/api/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-13 07:17:25.000000 codecarbon-2.2.1/carbonserver/carbonserver/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:17:41.178660 codecarbon-2.2.1/carbonserver/carbonserver/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:17:25.000000 codecarbon-2.2.1/carbonserver/carbonserver/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-13 07:17:25.000000 codecarbon-2.2.1/carbonserver/carbonserver/database/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-13 07:17:25.000000 codecarbon-2.2.1/carbonserver/carbonserver/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-05-13 07:17:25.000000 codecarbon-2.2.1/carbonserver/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-13 07:17:25.000000 codecarbon-2.2.1/carbonserver/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-13 07:17:25.000000 codecarbon-2.2.1/carbonserver/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:17:41.178660 codecarbon-2.2.1/codecarbon/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:17:41.182661 codecarbon-2.2.1/codecarbon/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/cli/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:17:41.182661 codecarbon-2.2.1/codecarbon/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/core/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/core/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/core/co2_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13758 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/core/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/core/emissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/core/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/core/rapl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/core/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/core/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/core/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:17:41.166660 codecarbon-2.2.1/codecarbon/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:17:41.182661 codecarbon-2.2.1/codecarbon/data/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/data/cloud/impact.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:17:41.186661 codecarbon-2.2.1/codecarbon/data/hardware/
--rw-r--r--   0 runner    (1001) docker     (123)    49423 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/data/hardware/cpu_power.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:17:41.186661 codecarbon-2.2.1/codecarbon/data/private_infra/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:17:41.186661 codecarbon-2.2.1/codecarbon/data/private_infra/2016/
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/data/private_infra/2016/canada_energy_mix.json
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/data/private_infra/2016/usa_emissions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/data/private_infra/carbon_intensity_per_source.json
--rw-r--r--   0 runner    (1001) docker     (123)    81313 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/data/private_infra/global_energy_mix.json
--rw-r--r--   0 runner    (1001) docker     (123)    37320 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/emissions_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:17:41.186661 codecarbon-2.2.1/codecarbon/external/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/external/geography.py
--rw-r--r--   0 runner    (1001) docker     (123)    11030 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/external/hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/external/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/external/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:17:41.190661 codecarbon-2.2.1/codecarbon/viz/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/viz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:17:41.190661 codecarbon-2.2.1/codecarbon/viz/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/viz/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25442 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/viz/assets/car_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    29734 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/viz/assets/house_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    29874 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/viz/assets/tv_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/viz/carbonboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/viz/carbonboard_on_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27905 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/viz/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    11230 2023-05-13 07:17:25.000000 codecarbon-2.2.1/codecarbon/viz/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:17:41.178660 codecarbon-2.2.1/codecarbon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-05-13 07:17:41.000000 codecarbon-2.2.1/codecarbon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-05-13 07:17:41.000000 codecarbon-2.2.1/codecarbon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 07:17:41.000000 codecarbon-2.2.1/codecarbon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-13 07:17:41.000000 codecarbon-2.2.1/codecarbon.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-13 07:17:41.000000 codecarbon-2.2.1/codecarbon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-13 07:17:41.000000 codecarbon-2.2.1/codecarbon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 07:17:41.198661 codecarbon-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-13 07:17:25.000000 codecarbon-2.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:17:41.194661 codecarbon-2.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-13 07:17:25.000000 codecarbon-2.2.1/tests/test_api_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-13 07:17:25.000000 codecarbon-2.2.1/tests/test_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-13 07:17:25.000000 codecarbon-2.2.1/tests/test_co2_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-05-13 07:17:25.000000 codecarbon-2.2.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-13 07:17:25.000000 codecarbon-2.2.1/tests/test_core_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10298 2023-05-13 07:17:25.000000 codecarbon-2.2.1/tests/test_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-05-13 07:17:25.000000 codecarbon-2.2.1/tests/test_emissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12810 2023-05-13 07:17:25.000000 codecarbon-2.2.1/tests/test_emissions_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-13 07:17:25.000000 codecarbon-2.2.1/tests/test_emissions_tracker_constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-13 07:17:25.000000 codecarbon-2.2.1/tests/test_emissions_tracker_flush.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-13 07:17:25.000000 codecarbon-2.2.1/tests/test_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-13 07:17:25.000000 codecarbon-2.2.1/tests/test_geography.py
--rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-05-13 07:17:25.000000 codecarbon-2.2.1/tests/test_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-13 07:17:25.000000 codecarbon-2.2.1/tests/test_hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-13 07:17:25.000000 codecarbon-2.2.1/tests/test_logging_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-13 07:17:25.000000 codecarbon-2.2.1/tests/test_ram.py
--rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-05-13 07:17:25.000000 codecarbon-2.2.1/tests/testdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-13 07:17:25.000000 codecarbon-2.2.1/tests/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.938085 codecarbon-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-25 09:25:41.000000 codecarbon-2.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-05-25 09:25:54.938085 codecarbon-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-05-25 09:25:41.000000 codecarbon-2.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.926085 codecarbon-2.2.2/carbonserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.926085 codecarbon-2.2.2/carbonserver/carbonserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.926085 codecarbon-2.2.2/carbonserver/carbonserver/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.930085 codecarbon-2.2.2/carbonserver/carbonserver/api/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/domain/emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/domain/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/domain/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/domain/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/domain/runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/domain/teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/domain/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.930085 codecarbon-2.2.2/carbonserver/carbonserver/api/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/routers/authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/routers/emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/routers/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/routers/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/routers/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/routers/runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/routers/teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/routers/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/api/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.930085 codecarbon-2.2.2/carbonserver/carbonserver/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/database/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/carbonserver/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-25 09:25:41.000000 codecarbon-2.2.2/carbonserver/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.930085 codecarbon-2.2.2/codecarbon/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.930085 codecarbon-2.2.2/codecarbon/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/cli/cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.934085 codecarbon-2.2.2/codecarbon/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/core/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/core/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/core/co2_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13758 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/core/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/core/emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/core/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/core/rapl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/core/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/core/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/core/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.926085 codecarbon-2.2.2/codecarbon/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.934085 codecarbon-2.2.2/codecarbon/data/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/data/cloud/impact.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.934085 codecarbon-2.2.2/codecarbon/data/hardware/
+-rw-r--r--   0 runner    (1001) docker     (123)    49423 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/data/hardware/cpu_power.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.934085 codecarbon-2.2.2/codecarbon/data/private_infra/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.934085 codecarbon-2.2.2/codecarbon/data/private_infra/2016/
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/data/private_infra/2016/canada_energy_mix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/data/private_infra/2016/usa_emissions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/data/private_infra/carbon_intensity_per_source.json
+-rw-r--r--   0 runner    (1001) docker     (123)   124501 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/data/private_infra/global_energy_mix.json
+-rw-r--r--   0 runner    (1001) docker     (123)    37361 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/emissions_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.934085 codecarbon-2.2.2/codecarbon/external/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/external/geography.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11030 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/external/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/external/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/external/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.934085 codecarbon-2.2.2/codecarbon/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/viz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.938085 codecarbon-2.2.2/codecarbon/viz/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/viz/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25442 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/viz/assets/car_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29734 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/viz/assets/house_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29874 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/viz/assets/tv_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/viz/carbonboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/viz/carbonboard_on_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27905 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/viz/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11230 2023-05-25 09:25:41.000000 codecarbon-2.2.2/codecarbon/viz/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.930085 codecarbon-2.2.2/codecarbon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-05-25 09:25:54.000000 codecarbon-2.2.2/codecarbon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-05-25 09:25:54.000000 codecarbon-2.2.2/codecarbon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:25:54.000000 codecarbon-2.2.2/codecarbon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-25 09:25:54.000000 codecarbon-2.2.2/codecarbon.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-25 09:25:54.000000 codecarbon-2.2.2/codecarbon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 09:25:54.000000 codecarbon-2.2.2/codecarbon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 09:25:54.938085 codecarbon-2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-25 09:25:41.000000 codecarbon-2.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:25:54.938085 codecarbon-2.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/test_api_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/test_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/test_co2_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/test_core_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10298 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/test_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/test_emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/test_emissions_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/test_emissions_tracker_constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/test_emissions_tracker_flush.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/test_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/test_geography.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/test_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/test_hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/test_logging_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/test_ram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/testdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-25 09:25:41.000000 codecarbon-2.2.2/tests/testutils.py
```

### Comparing `codecarbon-2.2.1/LICENSE` & `codecarbon-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/PKG-INFO` & `codecarbon-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codecarbon
-Version: 2.2.1
+Version: 2.2.2
 Author: Mila, DataForGood, BCG GAMMA, Comet.ml, Haverford College
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `codecarbon-2.2.1/README.md` & `codecarbon-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/carbonserver/carbonserver/api/dependencies.py` & `codecarbon-2.2.2/carbonserver/carbonserver/api/dependencies.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/carbonserver/carbonserver/api/domain/experiments.py` & `codecarbon-2.2.2/carbonserver/carbonserver/api/domain/experiments.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/carbonserver/carbonserver/api/errors.py` & `codecarbon-2.2.2/carbonserver/carbonserver/api/errors.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/carbonserver/carbonserver/api/routers/authenticate.py` & `codecarbon-2.2.2/carbonserver/carbonserver/api/routers/authenticate.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/carbonserver/carbonserver/api/routers/emissions.py` & `codecarbon-2.2.2/carbonserver/carbonserver/api/routers/emissions.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/carbonserver/carbonserver/api/routers/experiments.py` & `codecarbon-2.2.2/carbonserver/carbonserver/api/routers/experiments.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/carbonserver/carbonserver/api/routers/organizations.py` & `codecarbon-2.2.2/carbonserver/carbonserver/api/routers/organizations.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/carbonserver/carbonserver/api/routers/projects.py` & `codecarbon-2.2.2/carbonserver/carbonserver/api/routers/projects.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/carbonserver/carbonserver/api/routers/runs.py` & `codecarbon-2.2.2/carbonserver/carbonserver/api/routers/runs.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/carbonserver/carbonserver/api/routers/teams.py` & `codecarbon-2.2.2/carbonserver/carbonserver/api/routers/teams.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/carbonserver/carbonserver/api/routers/users.py` & `codecarbon-2.2.2/carbonserver/carbonserver/api/routers/users.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/carbonserver/carbonserver/api/schemas.py` & `codecarbon-2.2.2/carbonserver/carbonserver/api/schemas.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/carbonserver/carbonserver/database/database.py` & `codecarbon-2.2.2/carbonserver/carbonserver/database/database.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/carbonserver/container.py` & `codecarbon-2.2.2/carbonserver/container.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/carbonserver/main.py` & `codecarbon-2.2.2/carbonserver/main.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/carbonserver/setup.py` & `codecarbon-2.2.2/carbonserver/setup.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/codecarbon/cli/cli_utils.py` & `codecarbon-2.2.2/codecarbon/cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/codecarbon/cli/main.py` & `codecarbon-2.2.2/codecarbon/cli/main.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/codecarbon/core/api_client.py` & `codecarbon-2.2.2/codecarbon/core/api_client.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/codecarbon/core/cloud.py` & `codecarbon-2.2.2/codecarbon/core/cloud.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/codecarbon/core/co2_signal.py` & `codecarbon-2.2.2/codecarbon/core/co2_signal.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/codecarbon/core/config.py` & `codecarbon-2.2.2/codecarbon/core/config.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/codecarbon/core/cpu.py` & `codecarbon-2.2.2/codecarbon/core/cpu.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/codecarbon/core/emissions.py` & `codecarbon-2.2.2/codecarbon/core/emissions.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,31 +20,55 @@
 class Emissions:
     def __init__(
         self, data_source: DataSource, co2_signal_api_token: Optional[str] = None
     ):
         self._data_source = data_source
         self._co2_signal_api_token = co2_signal_api_token
 
-    def get_cloud_emissions(self, energy: Energy, cloud: CloudMetadata) -> float:
+    def get_cloud_emissions(
+        self, energy: Energy, cloud: CloudMetadata, geo: GeoMetadata = None
+    ) -> float:
         """
         Computes emissions for cloud infra
         :param energy: Mean power consumption of the process (kWh)
         :param cloud: Region of compute
+        :param geo: Instance of GeoMetadata to fallback if we don't find cloud carbon intensity
         :return: CO2 emissions in kg
         """
 
         df: pd.DataFrame = self._data_source.get_cloud_emissions_data()
-
-        emissions_per_kWh: EmissionsPerKWh = EmissionsPerKWh.from_g_per_kWh(
-            df.loc[(df["provider"] == cloud.provider) & (df["region"] == cloud.region)][
-                "impact"
-            ].item()
-        )
-
-        return emissions_per_kWh.kgs_per_kWh * energy.kWh  # kgs
+        try:
+            emissions_per_kWh: EmissionsPerKWh = EmissionsPerKWh.from_g_per_kWh(
+                df.loc[
+                    (df["provider"] == cloud.provider) & (df["region"] == cloud.region)
+                ]["impact"].item()
+            )
+            emissions = emissions_per_kWh.kgs_per_kWh * energy.kWh  # kgs
+        except Exception as e:
+            logger.warning(
+                f"Cloud electricity carbon intensity for provider '{cloud.provider}' and region '{cloud.region}' not found, using country value instead. Error : {e}"
+            )
+            logger.warning(
+                "AWS and Azure do not provide any carbon intensity data. Only GCP does it."
+            )
+            if geo:
+                emissions = self.get_private_infra_emissions(
+                    energy, geo
+                )  # float: kg co2_eq
+            else:
+                carbon_intensity_per_source = (
+                    DataSource().get_carbon_intensity_per_source_data()
+                )
+                emissions = (
+                    EmissionsPerKWh.from_g_per_kWh(
+                        carbon_intensity_per_source.get("world_average")
+                    ).kgs_per_kWh
+                    * energy.kWh
+                )  # kgs
+        return emissions
 
     def get_cloud_country_name(self, cloud: CloudMetadata) -> str:
         """
         Returns the Country Name where the cloud region is located
         """
         df: pd.DataFrame = self._data_source.get_cloud_emissions_data()
         return df.loc[
```

### Comparing `codecarbon-2.2.1/codecarbon/core/gpu.py` & `codecarbon-2.2.2/codecarbon/core/gpu.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/codecarbon/core/rapl.py` & `codecarbon-2.2.2/codecarbon/core/rapl.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/codecarbon/core/schemas.py` & `codecarbon-2.2.2/codecarbon/core/schemas.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/codecarbon/core/units.py` & `codecarbon-2.2.2/codecarbon/core/units.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/codecarbon/core/util.py` & `codecarbon-2.2.2/codecarbon/core/util.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/codecarbon/data/hardware/cpu_power.csv` & `codecarbon-2.2.2/codecarbon/data/hardware/cpu_power.csv`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/codecarbon/data/private_infra/2016/canada_energy_mix.json` & `codecarbon-2.2.2/codecarbon/data/private_infra/2016/canada_energy_mix.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/codecarbon/data/private_infra/2016/usa_emissions.json` & `codecarbon-2.2.2/codecarbon/data/private_infra/2016/usa_emissions.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/codecarbon/data/private_infra/carbon_intensity_per_source.json` & `codecarbon-2.2.2/codecarbon/data/private_infra/carbon_intensity_per_source.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/codecarbon/emissions_tracker.py` & `codecarbon-2.2.2/codecarbon/emissions_tracker.py`

 * *Files 0% similar despite different names*

```diff
@@ -458,15 +458,17 @@
             country_name = self._geo.country_name
             country_iso_code = self._geo.country_iso_code
             region = self._geo.region
             on_cloud = "N"
             cloud_provider = ""
             cloud_region = ""
         else:
-            emissions = self._emissions.get_cloud_emissions(self._total_energy, cloud)
+            emissions = self._emissions.get_cloud_emissions(
+                self._total_energy, cloud, self._geo
+            )
             country_name = self._emissions.get_cloud_country_name(cloud)
             country_iso_code = self._emissions.get_cloud_country_iso_code(cloud)
             region = self._emissions.get_cloud_geo_region(cloud)
             on_cloud = "Y"
             cloud_provider = cloud.provider
             cloud_region = cloud.region
         total_emissions = EmissionsData(
```

### Comparing `codecarbon-2.2.1/codecarbon/external/geography.py` & `codecarbon-2.2.2/codecarbon/external/geography.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,15 +39,20 @@
         cloud_metadata: Dict = get_env_cloud_details()
 
         if cloud_metadata is None:
             return cls(provider=None, region=None)
 
         provider: str = cloud_metadata["provider"].lower()
         region: str = extract_region_for_provider.get(provider)(cloud_metadata)
-
+        if provider in ["aws", "azure"]:
+            logger.warning(
+                f"Cloud provider '{provider}' do not publish electricity carbon intensity. Using country value instead."
+            )
+            provider = None
+            region = None
         return cls(provider=provider, region=region)
 
 
 class GeoMetadata:
     def __init__(
         self,
         country_iso_code: str,
```

### Comparing `codecarbon-2.2.1/codecarbon/external/hardware.py` & `codecarbon-2.2.2/codecarbon/external/hardware.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/codecarbon/external/logger.py` & `codecarbon-2.2.2/codecarbon/external/logger.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/codecarbon/external/scheduler.py` & `codecarbon-2.2.2/codecarbon/external/scheduler.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/codecarbon/input.py` & `codecarbon-2.2.2/codecarbon/input.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/codecarbon/output.py` & `codecarbon-2.2.2/codecarbon/output.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/codecarbon/viz/assets/car_icon.png` & `codecarbon-2.2.2/codecarbon/viz/assets/car_icon.png`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/codecarbon/viz/assets/house_icon.png` & `codecarbon-2.2.2/codecarbon/viz/assets/house_icon.png`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/codecarbon/viz/assets/tv_icon.png` & `codecarbon-2.2.2/codecarbon/viz/assets/tv_icon.png`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/codecarbon/viz/carbonboard.py` & `codecarbon-2.2.2/codecarbon/viz/carbonboard.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/codecarbon/viz/carbonboard_on_api.py` & `codecarbon-2.2.2/codecarbon/viz/carbonboard_on_api.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/codecarbon/viz/components.py` & `codecarbon-2.2.2/codecarbon/viz/components.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/codecarbon/viz/data.py` & `codecarbon-2.2.2/codecarbon/viz/data.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/codecarbon.egg-info/PKG-INFO` & `codecarbon-2.2.2/codecarbon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codecarbon
-Version: 2.2.1
+Version: 2.2.2
 Author: Mila, DataForGood, BCG GAMMA, Comet.ml, Haverford College
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `codecarbon-2.2.1/codecarbon.egg-info/SOURCES.txt` & `codecarbon-2.2.2/codecarbon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/setup.py` & `codecarbon-2.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ]
 
 TEST_DEPENDENCIES = ["mock", "pytest", "responses", "tox", "numpy", "requests-mock"]
 
 
 setuptools.setup(
     name="codecarbon",
-    version="2.2.1",
+    version="2.2.2",
     author="Mila, DataForGood, BCG GAMMA, Comet.ml, Haverford College",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license_files=("LICENSE",),
     packages=setuptools.find_packages(
         exclude=["*.tests", "*.tests.*", "tests.*", "tests"]
     ),
```

### Comparing `codecarbon-2.2.1/tests/test_api_call.py` & `codecarbon-2.2.2/tests/test_api_call.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "cpu_count": 12,
     "cpu_model": "Intel(R) Core(TM) i7-8850H CPU @ 2.60GHz",
     "gpu_count": 4,
     "gpu_model": "NVIDIA",
     "longitude": -7.6174,
     "latitude": 33.5822,
     "region": "EUROPE",
-    "provider": "AWS",
+    "provider": "GCP",
     "ram_total_size": 83948.22,
     "tracking_mode": "Machine",
 }
 
 
 def test_call_api():
     with requests_mock.Mocker() as m:
```

### Comparing `codecarbon-2.2.1/tests/test_cloud.py` & `codecarbon-2.2.2/tests/test_cloud.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/tests/test_co2_signal.py` & `codecarbon-2.2.2/tests/test_co2_signal.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/tests/test_config.py` & `codecarbon-2.2.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/tests/test_core_util.py` & `codecarbon-2.2.2/tests/test_core_util.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/tests/test_cpu.py` & `codecarbon-2.2.2/tests/test_cpu.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/tests/test_emissions.py` & `codecarbon-2.2.2/tests/test_emissions.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,26 +19,26 @@
         emissions = self._emissions.get_cloud_emissions(
             Energy.from_energy(kWh=0.6),
             CloudMetadata(provider="aws", region="us-east-1"),
         )
 
         # THEN
         assert isinstance(emissions, float)
-        self.assertAlmostEqual(emissions, 0.22, places=2)
+        self.assertAlmostEqual(emissions, 0.285, places=2)
 
     def test_emissions_CLOUD_AZURE(self):
         # WHEN
         emissions = self._emissions.get_cloud_emissions(
             Energy.from_energy(kWh=1.5),
             CloudMetadata(provider="azure", region="eastus"),
         )
 
         # THEN
         assert isinstance(emissions, float)
-        self.assertAlmostEqual(emissions, 0.55, places=2)
+        self.assertAlmostEqual(emissions, 0.7125, places=2)
 
     def test_emissions_CLOUD_GCP(self):
         emissions = self._emissions.get_cloud_emissions(
             Energy.from_energy(kWh=0.01),
             CloudMetadata(provider="gcp", region="us-central1"),
         )
 
@@ -76,22 +76,15 @@
 
         emissions = self._emissions.get_private_infra_emissions(
             Energy.from_energy(kWh=1_000),
             GeoMetadata(country_iso_code="JOR", country_name="Jordan"),
         )
 
         # THEN
-        jor_carbon_intensity = 17.19636 / 19.380129999999998 * 635  # fossil
-        jor_carbon_intensity += 0.02277 / 19.380129999999998 * 26  # hydroelectricity
-        jor_carbon_intensity += 1.441 / 19.380129999999998 * 48  # solar
-        jor_carbon_intensity += 0.72 / 19.380129999999998 * 26  # wind
-        jor_carbon_intensity /= 1000  # convert from g_per_kWh to kgs_per_kWh
-        jor_emissions = (
-            jor_carbon_intensity * 1_000
-        )  # Emissions in Kgs of CO2 For 1 000 kWh of energy
+        jor_emissions = 399.909  # Emissions in Kgs of CO2 For 1 000 kWh of energy
         assert isinstance(emissions, float)
         self.assertAlmostEqual(emissions, jor_emissions, places=2)
 
     def test_get_emissions_PRIVATE_INFRA_NOR(self):
         """
         Norway utilises hydropower more than any other country around the globe
         """
@@ -99,15 +92,15 @@
         emissions = self._emissions.get_private_infra_emissions(
             Energy.from_energy(kWh=1),
             GeoMetadata(country_iso_code="NOR", country_name="Norway"),
         )
 
         # THEN
         assert isinstance(emissions, float)
-        self.assertAlmostEqual(emissions, 33.4 / 1_000, places=2)
+        self.assertAlmostEqual(emissions, 26.4 / 1_000, places=2)
 
     def test_get_emissions_PRIVATE_INFRA_USA_WITH_REGION(self):
         # WHEN
         emissions = self._emissions.get_private_infra_emissions(
             Energy.from_energy(kWh=0.3),
             GeoMetadata(
                 country_iso_code="USA", country_name="United States", region="Illinois"
```

### Comparing `codecarbon-2.2.1/tests/test_emissions_tracker.py` & `codecarbon-2.2.2/tests/test_emissions_tracker.py`

 * *Files 1% similar despite different names*

```diff
@@ -285,15 +285,15 @@
         )
         tracker.start()
         heavy_computation(run_time_secs=2)
         tracker.stop()
 
         emissions_df = pd.read_csv(self.emissions_file_path)
 
-        self.assertEqual("US", emissions_df["country_name"].values[0])
+        self.assertEqual("United States", emissions_df["country_name"].values[0])
         self.assertEqual("USA", emissions_df["country_iso_code"].values[0])
 
     def test_offline_tracker_invalid_headers(
         self,
         mock_setup_intel_cli,
         mock_log_values,
         mocked_get_gpu_details,
@@ -315,15 +315,15 @@
         emissions_backup_df = pd.read_csv(
             self.emissions_file_path.with_suffix(".csv.bak")
         )
 
         self.verify_output_file(self.emissions_file_path, 2)
         self.verify_output_file(self.emissions_file_path.with_suffix(".csv.bak"), 2)
 
-        self.assertEqual("US", emissions_df["country_name"].values[0])
+        self.assertEqual("United States", emissions_df["country_name"].values[0])
         self.assertEqual("Morocco", emissions_backup_df["country_name"].values[0])
 
     def test_offline_tracker_valid_headers(
         self,
         mock_setup_intel_cli,
         mock_log_values,
         mocked_get_gpu_details,
@@ -345,15 +345,15 @@
 
         self.verify_output_file(self.emissions_file_path, 3)
 
         print(emissions_df["cpu_power"].values[0])
 
         self.assertAlmostEqual(0.269999999999999, emissions_df["cpu_power"].values[0])
         self.assertEqual("Morocco", emissions_df["country_name"].values[0])
-        self.assertEqual("US", emissions_df["country_name"].values[1])
+        self.assertEqual("United States", emissions_df["country_name"].values[1])
 
     def verify_output_file(self, file_path: str, num_lines: int) -> None:
         with open(file_path, "r") as f:
             lines = [line.rstrip() for line in f]
         assert len(lines) == num_lines
 
     @responses.activate
@@ -401,10 +401,10 @@
         with OfflineEmissionsTracker(
             country_iso_code="USA", output_dir=self.temp_path
         ) as tracker:
             heavy_computation(run_time_secs=2)
 
         emissions_df = pd.read_csv(self.emissions_file_path)
 
-        self.assertEqual("US", emissions_df["country_name"].values[0])
+        self.assertEqual("United States", emissions_df["country_name"].values[0])
         self.assertEqual("USA", emissions_df["country_iso_code"].values[0])
         self.assertIsInstance(tracker.final_emissions, float)
```

### Comparing `codecarbon-2.2.1/tests/test_emissions_tracker_constant.py` & `codecarbon-2.2.2/tests/test_emissions_tracker_constant.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 import tempfile
 import time
 import unittest
 from unittest import mock
 
+import pandas as pd
+
 from codecarbon.core import cpu
 from codecarbon.emissions_tracker import (
     EmissionsTracker,
     OfflineEmissionsTracker,
     track_emissions,
 )
 
@@ -58,31 +60,29 @@
         self.assertNotEqual(emissions, 0.0)
         self.assertAlmostEqual(emissions, 6.262572537957655e-05, places=2)
         self.verify_output_file(self.emissions_file_path)
 
     @mock.patch.object(cpu.TDP, "_get_cpu_power_from_registry")
     def test_carbon_tracker_offline_constant_default_cpu_power(self, mock_tdp):
         # Same as test_carbon_tracker_offline_constant test but this time forcing the default cpu power
-        USER_INPUT_CPU_POWER = 1000
+        USER_INPUT_CPU_POWER = 1_000
         # Mock the output of tdp
         mock_tdp.return_value = None
         tracker = OfflineEmissionsTracker(
             country_iso_code="USA",
             output_dir=self.emissions_path,
             output_file=self.emissions_file,
             default_cpu_power=USER_INPUT_CPU_POWER,
         )
         tracker.start()
         heavy_computation(run_time_secs=1)
         emissions = tracker.stop()
         assert isinstance(emissions, float)
         self.assertNotEqual(emissions, 0.0)
         # Assert the content stored. cpu_power should be 50% of input TDP
-        import pandas as pd
-
         assertdf = pd.read_csv(self.emissions_file_path)
         self.assertEqual(USER_INPUT_CPU_POWER / 2, assertdf["cpu_power"][0])
 
     def test_decorator_constant(self):
         @track_emissions(
             project_name=self.project_name,
             output_dir=self.emissions_path,
```

### Comparing `codecarbon-2.2.1/tests/test_emissions_tracker_flush.py` & `codecarbon-2.2.2/tests/test_emissions_tracker_flush.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/tests/test_energy.py` & `codecarbon-2.2.2/tests/test_energy.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/tests/test_geography.py` & `codecarbon-2.2.2/tests/test_geography.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,28 +19,34 @@
         return_value=CLOUD_METADATA_AWS,
     )
     def test_cloud_metadata_AWS(self, mock_get_env_cloud_details):
         # WHEN
         cloud = CloudMetadata.from_utils()
 
         # THEN
-        self.assertEqual("aws", cloud.provider)
-        self.assertEqual("us-east-1", cloud.region)
+        # AWS in not considered a cloud provider for CodeCarbon as it does not provide carbon intensity
+        # self.assertEqual("aws", cloud.provider)
+        # self.assertEqual("us-east-1", cloud.region)
+        self.assertEqual(None, cloud.provider)
+        self.assertEqual(None, cloud.region)
 
     @mock.patch(
         "codecarbon.external.geography.get_env_cloud_details",
         return_value=CLOUD_METADATA_AZURE,
     )
     def test_cloud_metadata_AZURE(self, mock_get_env_cloud_details):
         # WHEN
         cloud = CloudMetadata.from_utils()
 
         # THEN
-        self.assertEqual("azure", cloud.provider)
-        self.assertEqual("eastus", cloud.region)
+        # Azure in not considered a cloud provider for CodeCarbon as it does not provide carbon intensity
+        # self.assertEqual("azure", cloud.provider)
+        # self.assertEqual("eastus", cloud.region)
+        self.assertEqual(None, cloud.provider)
+        self.assertEqual(None, cloud.region)
 
     @mock.patch(
         "codecarbon.external.geography.get_env_cloud_details",
         return_value=CLOUD_METADATA_GCP,
     )
     def test_cloud_metadata_GCP(self, mock_get_env_cloud_details):
         # WHEN
```

### Comparing `codecarbon-2.2.1/tests/test_gpu.py` & `codecarbon-2.2.2/tests/test_gpu.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/tests/test_hardware.py` & `codecarbon-2.2.2/tests/test_hardware.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/tests/test_logging_output.py` & `codecarbon-2.2.2/tests/test_logging_output.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/tests/test_ram.py` & `codecarbon-2.2.2/tests/test_ram.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/tests/testdata.py` & `codecarbon-2.2.2/tests/testdata.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.2.1/tests/testutils.py` & `codecarbon-2.2.2/tests/testutils.py`

 * *Files identical despite different names*

