# Comparing `tmp/chime_frb_api-3.1.1.tar.gz` & `tmp/chime_frb_api-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chime_frb_api-3.1.1.tar", max compression
+gzip compressed data, was "chime_frb_api-3.2.0.tar", max compression
```

## Comparing `chime_frb_api-3.1.1.tar` & `chime_frb_api-3.2.0.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0     1080 2023-05-23 20:57:29.575793 chime_frb_api-3.1.1/LICENSE
--rw-r--r--   0        0        0     1386 2023-05-23 20:57:29.575793 chime_frb_api-3.1.1/README.md
--rw-r--r--   0        0        0      277 2023-05-23 20:57:29.575793 chime_frb_api-3.1.1/chime_frb_api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 20:57:29.575793 chime_frb_api-3.1.1/chime_frb_api/backends/__init__.py
--rw-r--r--   0        0        0      352 2023-05-23 20:57:29.575793 chime_frb_api-3.1.1/chime_frb_api/backends/bucket.py
--rw-r--r--   0        0        0      392 2023-05-23 20:57:29.575793 chime_frb_api-3.1.1/chime_frb_api/backends/distributor.py
--rw-r--r--   0        0        0     1932 2023-05-23 20:57:29.575793 chime_frb_api-3.1.1/chime_frb_api/backends/frb_master.py
--rw-r--r--   0        0        0      784 2023-05-23 20:57:29.575793 chime_frb_api-3.1.1/chime_frb_api/cli.py
--rw-r--r--   0        0        0      368 2023-05-23 20:57:29.575793 chime_frb_api-3.1.1/chime_frb_api/configs/__init__.py
--rw-r--r--   0        0        0      136 2023-05-23 20:57:29.575793 chime_frb_api-3.1.1/chime_frb_api/configs/test_workflow.yaml
--rw-r--r--   0        0        0     1185 2023-05-23 20:57:29.575793 chime_frb_api-3.1.1/chime_frb_api/configs/workflow.yaml
--rw-r--r--   0        0        0       48 2023-05-23 20:57:29.575793 chime_frb_api-3.1.1/chime_frb_api/core/__init__.py
--rw-r--r--   0        0        0    18785 2023-05-23 20:57:29.575793 chime_frb_api-3.1.1/chime_frb_api/core/core.py
--rw-r--r--   0        0        0      289 2023-05-23 20:57:29.575793 chime_frb_api-3.1.1/chime_frb_api/core/exceptions.py
--rw-r--r--   0        0        0      144 2023-05-23 20:57:29.575793 chime_frb_api-3.1.1/chime_frb_api/core/json_type.py
--rw-r--r--   0        0        0     2569 2023-05-23 20:57:29.575793 chime_frb_api-3.1.1/chime_frb_api/core/logger.py
--rw-r--r--   0        0        0      265 2023-05-23 20:57:29.575793 chime_frb_api-3.1.1/chime_frb_api/modules/__init__.py
--rw-r--r--   0        0        0     4193 2023-05-23 20:57:29.575793 chime_frb_api-3.1.1/chime_frb_api/modules/bucket.py
--rw-r--r--   0        0        0     8351 2023-05-23 20:57:29.575793 chime_frb_api-3.1.1/chime_frb_api/modules/buckets.py
--rw-r--r--   0        0        0     4548 2023-05-23 20:57:29.575793 chime_frb_api-3.1.1/chime_frb_api/modules/calibration.py
--rw-r--r--   0        0        0      570 2023-05-23 20:57:29.575793 chime_frb_api-3.1.1/chime_frb_api/modules/candidates.py
--rw-r--r--   0        0        0      810 2023-05-23 20:57:29.575793 chime_frb_api-3.1.1/chime_frb_api/modules/catalog.py
--rw-r--r--   0        0        0     4839 2023-05-23 20:57:29.575793 chime_frb_api-3.1.1/chime_frb_api/modules/distributor.py
--rw-r--r--   0        0        0    11217 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/modules/events.py
--rw-r--r--   0        0        0     5521 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/modules/metrics.py
--rw-r--r--   0        0        0     2013 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/modules/mimic.py
--rw-r--r--   0        0        0     4000 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/modules/parameters.py
--rw-r--r--   0        0        0     4882 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/modules/results.py
--rw-r--r--   0        0        0     1875 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/modules/sources.py
--rw-r--r--   0        0        0    11581 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/modules/swarm.py
--rw-r--r--   0        0        0    12551 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/modules/tns.py
--rw-r--r--   0        0        0     1879 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/modules/verification.py
--rw-r--r--   0        0        0    12214 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/modules/voe.py
--rw-r--r--   0        0        0     4234 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/modules/voe_subscribers.py
--rw-r--r--   0        0        0        0 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/stations/__init__.py
--rw-r--r--   0        0        0       22 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/stations/aro.py
--rw-r--r--   0        0        0      706 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/stations/drao.py
--rw-r--r--   0        0        0       22 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/stations/gbo.py
--rw-r--r--   0        0        0     2876 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/tests/docker-compose.yml
--rw-r--r--   0        0        0     9065 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/tests/test_archive.py
--rw-r--r--   0        0        0     3423 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/tests/test_audit_daemon.py
--rw-r--r--   0        0        0     1830 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/tests/test_bucket.py
--rw-r--r--   0        0        0     4282 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/tests/test_buckets.py
--rw-r--r--   0        0        0     1764 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/tests/test_calibration.py
--rw-r--r--   0        0        0      262 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/tests/test_candidates.py
--rw-r--r--   0        0        0      610 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/tests/test_catalog.py
--rw-r--r--   0        0        0     3413 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/tests/test_core.py
--rw-r--r--   0        0        0     2066 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/tests/test_distributor.py
--rw-r--r--   0        0        0     5823 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/tests/test_events.py
--rw-r--r--   0        0        0     3335 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/tests/test_metrics.py
--rw-r--r--   0        0        0      960 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/tests/test_mimic.py
--rw-r--r--   0        0        0      849 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/tests/test_parameters.py
--rw-r--r--   0        0        0     2134 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/tests/test_results.py
--rw-r--r--   0        0        0      384 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/tests/test_sources.py
--rw-r--r--   0        0        0      256 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/tests/test_stations.py
--rw-r--r--   0        0        0     1454 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/tests/test_swarm.py
--rw-r--r--   0        0        0     7035 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/tests/test_tns.py
--rw-r--r--   0        0        0     5367 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/tests/test_transfer_daemon.py
--rw-r--r--   0        0        0      467 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/tests/test_verification.py
--rw-r--r--   0        0        0     8503 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/tests/test_voe.py
--rw-r--r--   0        0        0     2780 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/tests/test_voe_subscribers.py
--rw-r--r--   0        0        0     5167 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/tests/test_work.py
--rw-r--r--   0        0        0     1208 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/tests/test_work_http_operations.py
--rw-r--r--   0        0        0     6650 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/tests/test_workflow.py
--rw-r--r--   0        0        0        0 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/utils/__init__.py
--rw-r--r--   0        0        0     2642 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/utils/copy.py
--rw-r--r--   0        0        0      859 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/utils/github.py
--rw-r--r--   0        0        0     1263 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/utils/loki.py
--rw-r--r--   0        0        0     2642 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/utils/move.py
--rw-r--r--   0        0        0       76 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/workflow/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/workflow/cli/__init__.py
--rw-r--r--   0        0        0     3951 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/workflow/cli/buckets.py
--rw-r--r--   0        0        0     5239 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/workflow/cli/pipelines.py
--rw-r--r--   0        0        0     9107 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/workflow/cli/run.py
--rw-r--r--   0        0        0      789 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/workflow/cli/sample.py
--rw-r--r--   0        0        0      671 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/workflow/cli/sample.yaml
--rw-r--r--   0        0        0        0 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/workflow/daemons/__init__.py
--rw-r--r--   0        0        0      980 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/workflow/daemons/audit.py
--rw-r--r--   0        0        0     6787 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/workflow/daemons/transfer.py
--rw-r--r--   0        0        0       32 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/workflow/lifecycle/__init__.py
--rw-r--r--   0        0        0     5166 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/workflow/lifecycle/archive.py
--rw-r--r--   0        0        0       33 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/workflow/lifecycle/attempt.py
--rw-r--r--   0        0        0      523 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/workflow/lifecycle/container.py
--rw-r--r--   0        0        0     4323 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/workflow/lifecycle/execute.py
--rw-r--r--   0        0        0     1418 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/workflow/lifecycle/validate.py
--rwxr-xr-x   0        0        0      408 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/workflow/runner.py
--rw-r--r--   0        0        0    18186 2023-05-23 20:57:29.579793 chime_frb_api-3.1.1/chime_frb_api/workflow/work.py
--rw-r--r--   0        0        0     1798 2023-05-23 20:57:29.599794 chime_frb_api-3.1.1/pyproject.toml
--rw-r--r--   0        0        0     2990 1970-01-01 00:00:00.000000 chime_frb_api-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-05-25 15:09:33.417735 chime_frb_api-3.2.0/LICENSE
+-rw-r--r--   0        0        0     1386 2023-05-25 15:09:33.417735 chime_frb_api-3.2.0/README.md
+-rw-r--r--   0        0        0      277 2023-05-25 15:09:33.417735 chime_frb_api-3.2.0/chime_frb_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-25 15:09:33.417735 chime_frb_api-3.2.0/chime_frb_api/backends/__init__.py
+-rw-r--r--   0        0        0      352 2023-05-25 15:09:33.417735 chime_frb_api-3.2.0/chime_frb_api/backends/bucket.py
+-rw-r--r--   0        0        0      392 2023-05-25 15:09:33.417735 chime_frb_api-3.2.0/chime_frb_api/backends/distributor.py
+-rw-r--r--   0        0        0     1932 2023-05-25 15:09:33.417735 chime_frb_api-3.2.0/chime_frb_api/backends/frb_master.py
+-rw-r--r--   0        0        0      784 2023-05-25 15:09:33.417735 chime_frb_api-3.2.0/chime_frb_api/cli.py
+-rw-r--r--   0        0        0      368 2023-05-25 15:09:33.417735 chime_frb_api-3.2.0/chime_frb_api/configs/__init__.py
+-rw-r--r--   0        0        0      136 2023-05-25 15:09:33.417735 chime_frb_api-3.2.0/chime_frb_api/configs/test_workflow.yaml
+-rw-r--r--   0        0        0     1185 2023-05-25 15:09:33.417735 chime_frb_api-3.2.0/chime_frb_api/configs/workflow.yaml
+-rw-r--r--   0        0        0       48 2023-05-25 15:09:33.417735 chime_frb_api-3.2.0/chime_frb_api/core/__init__.py
+-rw-r--r--   0        0        0    18785 2023-05-25 15:09:33.417735 chime_frb_api-3.2.0/chime_frb_api/core/core.py
+-rw-r--r--   0        0        0      289 2023-05-25 15:09:33.417735 chime_frb_api-3.2.0/chime_frb_api/core/exceptions.py
+-rw-r--r--   0        0        0      144 2023-05-25 15:09:33.417735 chime_frb_api-3.2.0/chime_frb_api/core/json_type.py
+-rw-r--r--   0        0        0     2569 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/core/logger.py
+-rw-r--r--   0        0        0      265 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/__init__.py
+-rw-r--r--   0        0        0     4193 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/bucket.py
+-rw-r--r--   0        0        0     8685 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/buckets.py
+-rw-r--r--   0        0        0     4548 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/calibration.py
+-rw-r--r--   0        0        0      570 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/candidates.py
+-rw-r--r--   0        0        0      810 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/catalog.py
+-rw-r--r--   0        0        0     4839 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/distributor.py
+-rw-r--r--   0        0        0    11217 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/events.py
+-rw-r--r--   0        0        0     5521 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/metrics.py
+-rw-r--r--   0        0        0     2013 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/mimic.py
+-rw-r--r--   0        0        0     4000 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/parameters.py
+-rw-r--r--   0        0        0     4882 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/results.py
+-rw-r--r--   0        0        0     1875 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/sources.py
+-rw-r--r--   0        0        0    11581 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/swarm.py
+-rw-r--r--   0        0        0    12551 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/tns.py
+-rw-r--r--   0        0        0     1879 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/verification.py
+-rw-r--r--   0        0        0    12214 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/voe.py
+-rw-r--r--   0        0        0     4234 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/modules/voe_subscribers.py
+-rw-r--r--   0        0        0        0 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/stations/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/stations/aro.py
+-rw-r--r--   0        0        0      706 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/stations/drao.py
+-rw-r--r--   0        0        0       22 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/stations/gbo.py
+-rw-r--r--   0        0        0     2876 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/docker-compose.yml
+-rw-r--r--   0        0        0     9065 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_archive.py
+-rw-r--r--   0        0        0     3423 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_audit_daemon.py
+-rw-r--r--   0        0        0     1830 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_bucket.py
+-rw-r--r--   0        0        0     4282 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_buckets.py
+-rw-r--r--   0        0        0     1764 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_calibration.py
+-rw-r--r--   0        0        0      262 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_candidates.py
+-rw-r--r--   0        0        0      610 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_catalog.py
+-rw-r--r--   0        0        0     3413 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_core.py
+-rw-r--r--   0        0        0     2066 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_distributor.py
+-rw-r--r--   0        0        0     5823 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_events.py
+-rw-r--r--   0        0        0     3335 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_metrics.py
+-rw-r--r--   0        0        0      960 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_mimic.py
+-rw-r--r--   0        0        0      849 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_parameters.py
+-rw-r--r--   0        0        0     2134 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_results.py
+-rw-r--r--   0        0        0      384 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_sources.py
+-rw-r--r--   0        0        0      256 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_stations.py
+-rw-r--r--   0        0        0     1454 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_swarm.py
+-rw-r--r--   0        0        0     7035 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_tns.py
+-rw-r--r--   0        0        0     5367 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_transfer_daemon.py
+-rw-r--r--   0        0        0      467 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_verification.py
+-rw-r--r--   0        0        0     8503 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_voe.py
+-rw-r--r--   0        0        0     2780 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_voe_subscribers.py
+-rw-r--r--   0        0        0     5167 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_work.py
+-rw-r--r--   0        0        0     1208 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_work_http_operations.py
+-rw-r--r--   0        0        0     6650 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/tests/test_workflow.py
+-rw-r--r--   0        0        0        0 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/utils/__init__.py
+-rw-r--r--   0        0        0     2642 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/utils/copy.py
+-rw-r--r--   0        0        0      859 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/utils/github.py
+-rw-r--r--   0        0        0     1263 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/utils/loki.py
+-rw-r--r--   0        0        0     2642 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/utils/move.py
+-rw-r--r--   0        0        0       76 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/cli/__init__.py
+-rw-r--r--   0        0        0     3899 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/cli/buckets.py
+-rw-r--r--   0        0        0     5239 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/cli/pipelines.py
+-rw-r--r--   0        0        0    10180 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/cli/run.py
+-rw-r--r--   0        0        0      789 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/cli/sample.py
+-rw-r--r--   0        0        0      671 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/cli/sample.yaml
+-rw-r--r--   0        0        0        0 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/daemons/__init__.py
+-rw-r--r--   0        0        0      980 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/daemons/audit.py
+-rw-r--r--   0        0        0     6787 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/daemons/transfer.py
+-rw-r--r--   0        0        0       32 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/lifecycle/__init__.py
+-rw-r--r--   0        0        0     5166 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/lifecycle/archive.py
+-rw-r--r--   0        0        0       33 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/lifecycle/attempt.py
+-rw-r--r--   0        0        0      523 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/lifecycle/container.py
+-rw-r--r--   0        0        0     4323 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/lifecycle/execute.py
+-rw-r--r--   0        0        0     1418 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/lifecycle/validate.py
+-rwxr-xr-x   0        0        0      408 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/runner.py
+-rw-r--r--   0        0        0    18365 2023-05-25 15:09:33.421735 chime_frb_api-3.2.0/chime_frb_api/workflow/work.py
+-rw-r--r--   0        0        0     1798 2023-05-25 15:09:33.437735 chime_frb_api-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2990 1970-01-01 00:00:00.000000 chime_frb_api-3.2.0/PKG-INFO
```

### Comparing `chime_frb_api-3.1.1/LICENSE` & `chime_frb_api-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/README.md` & `chime_frb_api-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/backends/frb_master.py` & `chime_frb_api-3.2.0/chime_frb_api/backends/frb_master.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/cli.py` & `chime_frb_api-3.2.0/chime_frb_api/cli.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/configs/workflow.yaml` & `chime_frb_api-3.2.0/chime_frb_api/configs/workflow.yaml`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/core/core.py` & `chime_frb_api-3.2.0/chime_frb_api/core/core.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/core/logger.py` & `chime_frb_api-3.2.0/chime_frb_api/core/logger.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/modules/bucket.py` & `chime_frb_api-3.2.0/chime_frb_api/modules/bucket.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/modules/buckets.py` & `chime_frb_api-3.2.0/chime_frb_api/modules/buckets.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,36 +64,44 @@
     def withdraw(
         self,
         pipeline: str,
         event: Optional[List[int]] = None,
         site: Optional[str] = None,
         priority: Optional[int] = None,
         user: Optional[str] = None,
+        tags: Optional[List[str]] = None,
+        parent: Optional[str] = None,
     ) -> Dict[str, Any]:
         """Withdraw `queued` work from the buckets backend.
 
         Args:
             pipeline (str): The pipeline to withdraw from. Required.
-            event (Optional[List[int]], optional): The event to withdraw from.
-            site (Optional[str], optional): The site to withdraw from.
+            event (Optional[List[int]], optional): The event to filter by.
+            site (Optional[str], optional): The site to filter by.
             priority (Optional[int], optional): The priority to withdraw from.
-            user (Optional[str], optional): The user to withdraw from.
+            user (Optional[str], optional): The user to filter by.
+            tags (Optional[List[str]], optional): The tags to filter by.
+            parent (Optional[str], optional): The parent to filter by.
 
         Returns:
             Dict[str, Any]: The work withdrawn.
         """
         query: Dict[str, Any] = {"pipeline": pipeline}
         if site:
             query["site"] = site
         if priority:
             query["priority"] = priority
         if user:
             query["user"] = user
         if event:
             query["event"] = {"$in": event}
+        if tags:
+            query["tags"] = {"$in": tags}
+        if parent:
+            query["config.parent"] = parent
         response: Dict[str, Any] = self.post(url="/work/withdraw", json=query)
         return response
 
     def update(self, works: List[Dict[str, Any]]) -> bool:
         """Update works in the buckets backend.
 
         Args:
```

### Comparing `chime_frb_api-3.1.1/chime_frb_api/modules/calibration.py` & `chime_frb_api-3.2.0/chime_frb_api/modules/calibration.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/modules/candidates.py` & `chime_frb_api-3.2.0/chime_frb_api/modules/candidates.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/modules/catalog.py` & `chime_frb_api-3.2.0/chime_frb_api/modules/catalog.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/modules/distributor.py` & `chime_frb_api-3.2.0/chime_frb_api/modules/distributor.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/modules/events.py` & `chime_frb_api-3.2.0/chime_frb_api/modules/events.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/modules/metrics.py` & `chime_frb_api-3.2.0/chime_frb_api/modules/metrics.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/modules/mimic.py` & `chime_frb_api-3.2.0/chime_frb_api/modules/mimic.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/modules/parameters.py` & `chime_frb_api-3.2.0/chime_frb_api/modules/parameters.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/modules/results.py` & `chime_frb_api-3.2.0/chime_frb_api/modules/results.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/modules/sources.py` & `chime_frb_api-3.2.0/chime_frb_api/modules/sources.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/modules/swarm.py` & `chime_frb_api-3.2.0/chime_frb_api/modules/swarm.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/modules/tns.py` & `chime_frb_api-3.2.0/chime_frb_api/modules/tns.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/modules/verification.py` & `chime_frb_api-3.2.0/chime_frb_api/modules/verification.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/modules/voe.py` & `chime_frb_api-3.2.0/chime_frb_api/modules/voe.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/modules/voe_subscribers.py` & `chime_frb_api-3.2.0/chime_frb_api/modules/voe_subscribers.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/stations/drao.py` & `chime_frb_api-3.2.0/chime_frb_api/stations/drao.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/tests/docker-compose.yml` & `chime_frb_api-3.2.0/chime_frb_api/tests/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/tests/test_archive.py` & `chime_frb_api-3.2.0/chime_frb_api/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/tests/test_audit_daemon.py` & `chime_frb_api-3.2.0/chime_frb_api/tests/test_audit_daemon.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/tests/test_bucket.py` & `chime_frb_api-3.2.0/chime_frb_api/tests/test_bucket.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/tests/test_buckets.py` & `chime_frb_api-3.2.0/chime_frb_api/tests/test_buckets.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/tests/test_calibration.py` & `chime_frb_api-3.2.0/chime_frb_api/tests/test_calibration.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/tests/test_catalog.py` & `chime_frb_api-3.2.0/chime_frb_api/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/tests/test_core.py` & `chime_frb_api-3.2.0/chime_frb_api/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/tests/test_distributor.py` & `chime_frb_api-3.2.0/chime_frb_api/tests/test_distributor.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/tests/test_events.py` & `chime_frb_api-3.2.0/chime_frb_api/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/tests/test_metrics.py` & `chime_frb_api-3.2.0/chime_frb_api/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/tests/test_mimic.py` & `chime_frb_api-3.2.0/chime_frb_api/tests/test_mimic.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/tests/test_parameters.py` & `chime_frb_api-3.2.0/chime_frb_api/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/tests/test_results.py` & `chime_frb_api-3.2.0/chime_frb_api/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/tests/test_swarm.py` & `chime_frb_api-3.2.0/chime_frb_api/tests/test_swarm.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/tests/test_tns.py` & `chime_frb_api-3.2.0/chime_frb_api/tests/test_tns.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/tests/test_transfer_daemon.py` & `chime_frb_api-3.2.0/chime_frb_api/tests/test_transfer_daemon.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/tests/test_voe.py` & `chime_frb_api-3.2.0/chime_frb_api/tests/test_voe.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/tests/test_voe_subscribers.py` & `chime_frb_api-3.2.0/chime_frb_api/tests/test_voe_subscribers.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/tests/test_work.py` & `chime_frb_api-3.2.0/chime_frb_api/tests/test_work.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/tests/test_work_http_operations.py` & `chime_frb_api-3.2.0/chime_frb_api/tests/test_work_http_operations.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/tests/test_workflow.py` & `chime_frb_api-3.2.0/chime_frb_api/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/utils/copy.py` & `chime_frb_api-3.2.0/chime_frb_api/utils/copy.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/utils/github.py` & `chime_frb_api-3.2.0/chime_frb_api/utils/github.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/utils/loki.py` & `chime_frb_api-3.2.0/chime_frb_api/utils/loki.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/utils/move.py` & `chime_frb_api-3.2.0/chime_frb_api/utils/move.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/workflow/cli/buckets.py` & `chime_frb_api-3.2.0/chime_frb_api/workflow/cli/buckets.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,26 +27,26 @@
 @buckets.command("version", help="Show the version.")
 def version():
     """Show the version."""
     buckets = Buckets()
     console.print(buckets.version())
 
 
-@buckets.command("prune", help="Prune work[s] from a workflow bucket.")
-@click.option("name", "--name", type=str, required=True, help="Name of the bucket.")
+@buckets.command("rm", help="Remove a bucket.")
+@click.argument("name", type=str, required=True)
 @click.option("event", "--event", type=int, required=False, help="CHIME/FRB Event ID.")
 @click.option(
     "status",
     "--status",
     type=str,
     required=False,
-    help="To prune work of particular status.",
+    help="Remove works with only a particular status.",
 )
 def prune_work(name: str, event: Optional[int] = None, status: Optional[str] = None):
-    """Prune work[s] from the workflow backend.
+    """Remove work[s] from the buckets backend.
 
     Args:
         name (str): Name of the workflow pipeline.
         event (Optional[int], optional): CHIME/FRB Event ID. Defaults to None.
         status (Optional[str], optional): Status of work[s] to prune. Defaults to None.
     """
     events: Optional[List[int]] = None
```

### Comparing `chime_frb_api-3.1.1/chime_frb_api/workflow/cli/pipelines.py` & `chime_frb_api-3.2.0/chime_frb_api/workflow/cli/pipelines.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/workflow/cli/run.py` & `chime_frb_api-3.2.0/chime_frb_api/workflow/cli/run.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Fetch and process Work using any method compatible with Tasks API."""
 
 
 import platform
 import signal
 import time
 from threading import Event
-from typing import Any, Callable, Dict, List, Optional
+from typing import Any, Callable, Dict, List, Optional, Tuple
 
 import click
 import requests
 from rich.console import Console
 
 from chime_frb_api import get_logger
 from chime_frb_api.configs import LOKI_URLS, PRODUCTS_URLS, WORKFLOW_URLS
@@ -35,14 +35,33 @@
         ["chime", "allenby", "kko", "gbo", "hco", "aro", "canfar", "cedar", "local"]
     ),
     required=True,
     show_default=True,
     help="filter work by site.",
 )
 @click.option(
+    "-t",
+    "--tag",
+    type=str,
+    multiple=True,
+    required=False,
+    default=None,
+    show_default=True,
+    help="filter work by tag, multiple values allowed.",
+)
+@click.option(
+    "-p",
+    "--parent",
+    type=str,
+    required=False,
+    default=None,
+    show_default=True,
+    help="filter work by parent pipeline.",
+)
+@click.option(
     "-c",
     "--command",
     type=str,
     required=False,
     default=None,
     show_default=True,
     help="command to perform, e.g. `ls -l`",
@@ -81,15 +100,15 @@
 )
 @click.option(
     "--products-url",
     type=click.STRING,
     default=None,
     required=False,
     show_default=True,
-    help="url for products and plotsj.",
+    help="url for products server.",
 )
 @click.option(
     "--log-level",
     type=click.Choice(["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]),
     default="INFO",
     show_default=True,
     help="logging level.",
@@ -98,43 +117,55 @@
     bucket: str,
     function: str,
     command: str,
     lifetime: int,
     sleep_time: int,
     base_url: Optional[str],
     site: str,
+    tag: Tuple[str],
+    parent: Optional[str],
     loki_url: Optional[str],
     products_url: Optional[str],
     log_level: str,
 ):
     """Perform work retrieved from the workflow buckets."""
     # Set logging level
     logger.root.setLevel(log_level)
     logger.root.handlers[0].setLevel(log_level)
     if not base_url:
         base_url = str(WORKFLOW_URLS[site])
     if not loki_url:
         loki_url = str(LOKI_URLS[site])
     if not products_url:
         products_url = str(PRODUCTS_URLS[site])
+    # Reformate tag to be a list of strings
+    tags: List[str] = list(tag)
     # Setup and connect to the workflow backend
     logger.info("[bold]Workflow Run CLI[/bold]", extra=dict(markup=True, color="green"))
     logger.info(f"Bucket   : {bucket}")
     logger.info(f"Function : {function}")
     logger.info(f"Command  : {command}")
     logger.info(f"Mode     : {'Static' if (function or command) else 'Dynamic'}")
     # Print inifinity symbol if lifetime is -1, otherwise print lifetime
     logger.info(f"Lifetime : {'infinite' if lifetime == -1 else lifetime}")
     logger.info(f"Sleep    : {sleep_time}s")
-    logger.info(f"Work Site: {site}")
     logger.info(f"Log Level: {log_level}")
     logger.info(f"Base URL : {base_url}")
     logger.info(f"Loki URL : {loki_url}")
     logger.info(f"Prod URL : {products_url}")
     logger.info(
+        "[bold red]Work Filters [/bold red]",
+        extra=dict(markup=True, color="green"),
+    )
+    logger.info(f"Site: {site}")
+    if tags:
+        logger.info(f"Tags: {tags}")
+    if parent:
+        logger.info(f"Parent Pipeline: {parent}")
+    logger.info(
         "[bold]Execution Environment [/bold]",
         extra=dict(markup=True, color="green"),
     )
     logger.info(f"Operating System: {platform.system()}")
     logger.info(f"Python Version  : {platform.python_version()}")
     logger.info(f"Python Compiler : {platform.python_compiler()}")
     logger.info(f"Virtualization  : {container.virtualization()}")
@@ -170,15 +201,17 @@
         with console.status(
             status="",
             spinner="toggle2",
             spinner_style="bold green",
             refresh_per_second=1,
             speed=1 / slowdown,
         ):
-            lifecycle(bucket, function, lifetime, sleep_time, site, base_url)
+            lifecycle(
+                bucket, function, lifetime, sleep_time, site, tags, parent, base_url
+            )
     except Exception as error:
         logger.exception(error)
     finally:
         logger.info(
             "[bold]Workflow Lifecycle Complete[/bold]",
             extra=dict(markup=True, color="green"),
         )
@@ -186,14 +219,16 @@
 
 def lifecycle(
     bucket: str,
     function: Optional[str],
     lifetime: int,
     sleep_time: int,
     site: str,
+    tags: List[str],
+    parent: Optional[str],
     base_url: str,
 ):
     """Run the workflow lifecycle."""
     # Start the exit event
     exit = Event()
 
     # Get any stop, kill, or terminate signals and set the exit event
@@ -204,29 +239,38 @@
 
     # Register the quit function to handle the signals
     for sig in ("TERM", "HUP", "INT"):
         signal.signal(getattr(signal, "SIG" + sig), quit)
 
     # Run the lifecycle until the exit event is set or the lifetime is reached
     while lifetime != 0 and not exit.is_set():
-        attempt(bucket, function, base_url, site)
+        attempt(bucket, function, base_url, site, tags, parent)
         lifetime -= 1
         logger.debug(f"sleeping: {sleep_time}s")
         exit.wait(sleep_time)
         logger.debug(f"awake: {sleep_time}s")
 
 
-def attempt(bucket: str, function: Optional[str], base_url: str, site: str) -> bool:
+def attempt(
+    bucket: str,
+    function: Optional[str],
+    base_url: str,
+    site: str,
+    tags: Optional[List[str]],
+    parent: Optional[str],
+) -> bool:
     """Attempt to perform work.
 
     Args:
         bucket (str): Name of the bucket to perform work from.
         function (Optional[str]): Static function to perform work.
         base_url (str): URL of the workflow backend.
         site (str): Site to filter work by.
+        tags (Optional[List[str]]): Tags to filter work by.
+        parent (Optional[str]): Parent pipeline to filter work by.
 
     Returns:
         bool: True if work was performed, False otherwise.
     """
     kwargs: Dict[str, Any] = {"base_url": base_url}
     mode: str = "dynamic"
     work: Optional[Work] = None
@@ -240,15 +284,17 @@
             user_func = validate.function(function)
         else:
             mode = "dynamic"
             user_func = None
 
         # Get work from the workflow backend
         try:
-            work = Work.withdraw(pipeline=bucket, site=site, **kwargs)
+            work = Work.withdraw(
+                pipeline=bucket, site=site, tags=tags, parent=parent, **kwargs
+            )
         except Exception as error:
             logger.exception(error)
 
         if work:
             # Set the work id for the logger
             set_tag(work.id)  # type: ignore
             logger.info("work retrieved: ✅")
```

### Comparing `chime_frb_api-3.1.1/chime_frb_api/workflow/cli/sample.py` & `chime_frb_api-3.2.0/chime_frb_api/workflow/cli/sample.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/workflow/cli/sample.yaml` & `chime_frb_api-3.2.0/chime_frb_api/workflow/cli/sample.yaml`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/workflow/daemons/audit.py` & `chime_frb_api-3.2.0/chime_frb_api/workflow/daemons/audit.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/workflow/daemons/transfer.py` & `chime_frb_api-3.2.0/chime_frb_api/workflow/daemons/transfer.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/workflow/lifecycle/archive.py` & `chime_frb_api-3.2.0/chime_frb_api/workflow/lifecycle/archive.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/workflow/lifecycle/container.py` & `chime_frb_api-3.2.0/chime_frb_api/workflow/lifecycle/container.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/workflow/lifecycle/execute.py` & `chime_frb_api-3.2.0/chime_frb_api/workflow/lifecycle/execute.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/workflow/lifecycle/validate.py` & `chime_frb_api-3.2.0/chime_frb_api/workflow/lifecycle/validate.py`

 * *Files identical despite different names*

### Comparing `chime_frb_api-3.1.1/chime_frb_api/workflow/work.py` & `chime_frb_api-3.2.0/chime_frb_api/workflow/work.py`

 * *Files 5% similar despite different names*

```diff
@@ -482,28 +482,36 @@
     def withdraw(
         cls,
         pipeline: str,
         event: Optional[List[int]] = None,
         site: Optional[str] = None,
         priority: Optional[int] = None,
         user: Optional[str] = None,
+        tags: Optional[List[str]] = None,
+        parent: Optional[str] = None,
         **kwargs: Dict[str, Any],
     ) -> Optional["Work"]:
         """Withdraw work from the buckets backend.
 
         Args:
             pipeline (str): Name of the pipeline.
             **kwargs (Dict[str, Any]): Keyword arguments for the Buckets API.
 
         Returns:
             Work: Work object.
         """
         buckets = Buckets(**kwargs)  # type: ignore
         payload = buckets.withdraw(
-            pipeline=pipeline, event=event, site=site, priority=priority, user=user
+            pipeline=pipeline,
+            event=event,
+            site=site,
+            priority=priority,
+            user=user,
+            tags=tags,
+            parent=parent,
         )
         if payload:
             return cls.from_dict(payload)
         return None
 
     @retry(wait=wait_random(min=0.5, max=1.5), stop=(stop_after_delay(30)))
     def deposit(
```

### Comparing `chime_frb_api-3.1.1/pyproject.toml` & `chime_frb_api-3.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chime-frb-api"
-version = "3.1.1"
+version = "3.2.0"
 description = "CHIME/FRB API"
 authors = ["Shiny Brar <charanjotbrar@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/CHIMEFRB/frb-api"
 documentation = "https://github.com/CHIMEFRB/frb-api"
 classifiers = [
```

### Comparing `chime_frb_api-3.1.1/PKG-INFO` & `chime_frb_api-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chime-frb-api
-Version: 3.1.1
+Version: 3.2.0
 Summary: CHIME/FRB API
 Home-page: https://github.com/CHIMEFRB/frb-api
 License: MIT
 Author: Shiny Brar
 Author-email: charanjotbrar@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

