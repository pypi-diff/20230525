# Comparing `tmp/dagster_cloud-1.3.5.tar.gz` & `tmp/dagster_cloud-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_cloud-1.3.5.tar", last modified: Thu May 18 20:49:47 2023, max compression
+gzip compressed data, was "dagster_cloud-1.3.6.tar", last modified: Thu May 25 17:28:00 2023, max compression
```

## Comparing `dagster_cloud-1.3.5.tar` & `dagster_cloud-1.3.6.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.381680 dagster_cloud-1.3.5/
--rw-r--r--   0 root         (0) root         (0)     4537 2023-05-18 20:49:47.381680 dagster_cloud-1.3.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3062 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.317680 dagster_cloud-1.3.5/dagster_cloud/
--rw-r--r--   0 root         (0) root         (0)      140 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.321680 dagster_cloud-1.3.5/dagster_cloud/agent/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.321680 dagster_cloud-1.3.5/dagster_cloud/agent/cli/
--rw-r--r--   0 root         (0) root         (0)     7584 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/agent/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43075 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/agent/dagster_cloud_agent.py
--rw-r--r--   0 root         (0) root         (0)     1578 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/agent/queries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.321680 dagster_cloud-1.3.5/dagster_cloud/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16984 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/api/dagster_cloud_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.325680 dagster_cloud-1.3.5/dagster_cloud/auth/
--rw-r--r--   0 root         (0) root         (0)      248 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1242 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/auth/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.325680 dagster_cloud-1.3.5/dagster_cloud/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/execution/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.333680 dagster_cloud-1.3.5/dagster_cloud/execution/cloud_run_launcher/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/execution/cloud_run_launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)      327 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/execution/cloud_run_launcher/k8s.py
--rw-r--r--   0 root         (0) root         (0)     3223 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/execution/cloud_run_launcher/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.333680 dagster_cloud-1.3.5/dagster_cloud/execution/monitoring/
--rw-r--r--   0 root         (0) root         (0)    14188 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/execution/monitoring/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.337680 dagster_cloud-1.3.5/dagster_cloud/execution/utils/
--rw-r--r--   0 root         (0) root         (0)      254 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/execution/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      875 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/execution/utils/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.337680 dagster_cloud-1.3.5/dagster_cloud/instance/
--rw-r--r--   0 root         (0) root         (0)    18147 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/instance/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.337680 dagster_cloud-1.3.5/dagster_cloud/pex/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/pex/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.341680 dagster_cloud-1.3.5/dagster_cloud/pex/grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.341680 dagster_cloud-1.3.5/dagster_cloud/pex/grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      285 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/pex/grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6822 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7786 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      327 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/pex/grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4541 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/pex/grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     4364 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/pex/grpc/compile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.345680 dagster_cloud-1.3.5/dagster_cloud/pex/grpc/server/
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/pex/grpc/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.345680 dagster_cloud-1.3.5/dagster_cloud/pex/grpc/server/cli/
--rw-r--r--   0 root         (0) root         (0)     1781 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/pex/grpc/server/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10312 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/pex/grpc/server/manager.py
--rw-r--r--   0 root         (0) root         (0)     9912 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/pex/grpc/server/registry.py
--rw-r--r--   0 root         (0) root         (0)    11492 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/pex/grpc/server/server.py
--rw-r--r--   0 root         (0) root         (0)     2889 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/pex/grpc/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.349680 dagster_cloud-1.3.5/dagster_cloud/secrets/
--rw-r--r--   0 root         (0) root         (0)       75 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1794 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.349680 dagster_cloud-1.3.5/dagster_cloud/serverless/
--rw-r--r--   0 root         (0) root         (0)       71 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/serverless/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4616 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/serverless/io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.349680 dagster_cloud-1.3.5/dagster_cloud/storage/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/storage/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.353680 dagster_cloud-1.3.5/dagster_cloud/storage/compute_logs/
--rw-r--r--   0 root         (0) root         (0)       82 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/storage/compute_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4582 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/storage/compute_logs/compute_log_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.357680 dagster_cloud-1.3.5/dagster_cloud/storage/event_logs/
--rw-r--r--   0 root         (0) root         (0)       70 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/storage/event_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9532 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/storage/event_logs/queries.py
--rw-r--r--   0 root         (0) root         (0)    26932 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/storage/event_logs/storage.py
--rw-r--r--   0 root         (0) root         (0)      658 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/storage/event_logs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.357680 dagster_cloud-1.3.5/dagster_cloud/storage/runs/
--rw-r--r--   0 root         (0) root         (0)       60 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6504 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/storage/runs/queries.py
--rw-r--r--   0 root         (0) root         (0)    19041 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/storage/runs/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.361680 dagster_cloud-1.3.5/dagster_cloud/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)       70 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1927 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/storage/schedules/queries.py
--rw-r--r--   0 root         (0) root         (0)     7209 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/storage/schedules/storage.py
--rw-r--r--   0 root         (0) root         (0)      280 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/storage/tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.361680 dagster_cloud-1.3.5/dagster_cloud/util/
--rw-r--r--   0 root         (0) root         (0)     2248 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.361680 dagster_cloud-1.3.5/dagster_cloud/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.365680 dagster_cloud-1.3.5/dagster_cloud/workspace/cli/
--rw-r--r--   0 root         (0) root         (0)     6948 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.365680 dagster_cloud-1.3.5/dagster_cloud/workspace/config_schema/
--rw-r--r--   0 root         (0) root         (0)     8613 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/config_schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)      967 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/config_schema/docker.py
--rw-r--r--   0 root         (0) root         (0)     4972 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/config_schema/ecs.py
--rw-r--r--   0 root         (0) root         (0)     6130 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/config_schema/kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.369680 dagster_cloud-1.3.5/dagster_cloud/workspace/docker/
--rw-r--r--   0 root         (0) root         (0)    12011 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/docker/__init__.py
--rw-r--r--   0 root         (0) root         (0)      327 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/docker/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.373680 dagster_cloud-1.3.5/dagster_cloud/workspace/ecs/
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/ecs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23263 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/ecs/client.py
--rw-r--r--   0 root         (0) root         (0)    21621 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/ecs/launcher.py
--rw-r--r--   0 root         (0) root         (0)      694 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/ecs/run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     4165 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/ecs/service.py
--rw-r--r--   0 root         (0) root         (0)     1748 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/ecs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.377680 dagster_cloud-1.3.5/dagster_cloud/workspace/kubernetes/
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/kubernetes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17127 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/kubernetes/launcher.py
--rw-r--r--   0 root         (0) root         (0)    11407 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/kubernetes/utils.py
--rw-r--r--   0 root         (0) root         (0)     1268 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/origin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.381680 dagster_cloud-1.3.5/dagster_cloud/workspace/user_code_launcher/
--rw-r--r--   0 root         (0) root         (0)      745 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/user_code_launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12807 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/user_code_launcher/process.py
--rw-r--r--   0 root         (0) root         (0)    74026 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1192 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/dagster_cloud/workspace/user_code_launcher/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:47.317680 dagster_cloud-1.3.5/dagster_cloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4537 2023-05-18 20:49:47.000000 dagster_cloud-1.3.5/dagster_cloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3216 2023-05-18 20:49:47.000000 dagster_cloud-1.3.5/dagster_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 20:49:47.000000 dagster_cloud-1.3.5/dagster_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-18 20:49:47.000000 dagster_cloud-1.3.5/dagster_cloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-05-18 20:49:47.000000 dagster_cloud-1.3.5/dagster_cloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-18 20:49:47.381680 dagster_cloud-1.3.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2890 2023-05-18 20:38:22.000000 dagster_cloud-1.3.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:00.946475 dagster_cloud-1.3.6/
+-rw-r--r--   0 root         (0) root         (0)     4537 2023-05-25 17:28:00.946475 dagster_cloud-1.3.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3062 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:00.886475 dagster_cloud-1.3.6/dagster_cloud/
+-rw-r--r--   0 root         (0) root         (0)      140 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:00.890475 dagster_cloud-1.3.6/dagster_cloud/agent/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:00.890475 dagster_cloud-1.3.6/dagster_cloud/agent/cli/
+-rw-r--r--   0 root         (0) root         (0)     7584 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/agent/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43075 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/agent/dagster_cloud_agent.py
+-rw-r--r--   0 root         (0) root         (0)     1578 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/agent/queries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:00.890475 dagster_cloud-1.3.6/dagster_cloud/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16984 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/api/dagster_cloud_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:00.894475 dagster_cloud-1.3.6/dagster_cloud/auth/
+-rw-r--r--   0 root         (0) root         (0)      248 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1242 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/auth/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:00.894475 dagster_cloud-1.3.6/dagster_cloud/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/execution/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:00.894475 dagster_cloud-1.3.6/dagster_cloud/execution/cloud_run_launcher/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/execution/cloud_run_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      327 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/execution/cloud_run_launcher/k8s.py
+-rw-r--r--   0 root         (0) root         (0)     3223 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/execution/cloud_run_launcher/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:00.894475 dagster_cloud-1.3.6/dagster_cloud/execution/monitoring/
+-rw-r--r--   0 root         (0) root         (0)    14188 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/execution/monitoring/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:00.898475 dagster_cloud-1.3.6/dagster_cloud/execution/utils/
+-rw-r--r--   0 root         (0) root         (0)      254 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/execution/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      875 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/execution/utils/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:00.898475 dagster_cloud-1.3.6/dagster_cloud/instance/
+-rw-r--r--   0 root         (0) root         (0)    18147 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/instance/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:00.898475 dagster_cloud-1.3.6/dagster_cloud/pex/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/pex/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:00.906475 dagster_cloud-1.3.6/dagster_cloud/pex/grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:00.906475 dagster_cloud-1.3.6/dagster_cloud/pex/grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      285 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/pex/grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6822 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7786 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      327 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/pex/grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4541 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/pex/grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     4364 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/pex/grpc/compile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:00.910475 dagster_cloud-1.3.6/dagster_cloud/pex/grpc/server/
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/pex/grpc/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:00.910475 dagster_cloud-1.3.6/dagster_cloud/pex/grpc/server/cli/
+-rw-r--r--   0 root         (0) root         (0)     1781 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/pex/grpc/server/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10312 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/pex/grpc/server/manager.py
+-rw-r--r--   0 root         (0) root         (0)     9912 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/pex/grpc/server/registry.py
+-rw-r--r--   0 root         (0) root         (0)    11492 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/pex/grpc/server/server.py
+-rw-r--r--   0 root         (0) root         (0)     2889 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/pex/grpc/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:00.914475 dagster_cloud-1.3.6/dagster_cloud/secrets/
+-rw-r--r--   0 root         (0) root         (0)       75 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1794 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:00.914475 dagster_cloud-1.3.6/dagster_cloud/serverless/
+-rw-r--r--   0 root         (0) root         (0)       71 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/serverless/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4616 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/serverless/io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:00.918475 dagster_cloud-1.3.6/dagster_cloud/storage/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/storage/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:00.918475 dagster_cloud-1.3.6/dagster_cloud/storage/compute_logs/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/storage/compute_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4582 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/storage/compute_logs/compute_log_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:00.922475 dagster_cloud-1.3.6/dagster_cloud/storage/event_logs/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/storage/event_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9532 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/storage/event_logs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    26988 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/storage/event_logs/storage.py
+-rw-r--r--   0 root         (0) root         (0)      658 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/storage/event_logs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:00.922475 dagster_cloud-1.3.6/dagster_cloud/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)       60 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6504 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/storage/runs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    19041 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/storage/runs/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:00.926475 dagster_cloud-1.3.6/dagster_cloud/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1927 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/storage/schedules/queries.py
+-rw-r--r--   0 root         (0) root         (0)     7209 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/storage/schedules/storage.py
+-rw-r--r--   0 root         (0) root         (0)      280 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/storage/tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:00.926475 dagster_cloud-1.3.6/dagster_cloud/util/
+-rw-r--r--   0 root         (0) root         (0)     2248 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:00.926475 dagster_cloud-1.3.6/dagster_cloud/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/workspace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:00.930475 dagster_cloud-1.3.6/dagster_cloud/workspace/cli/
+-rw-r--r--   0 root         (0) root         (0)     6948 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/workspace/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:00.930475 dagster_cloud-1.3.6/dagster_cloud/workspace/config_schema/
+-rw-r--r--   0 root         (0) root         (0)     8613 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/workspace/config_schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      967 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/workspace/config_schema/docker.py
+-rw-r--r--   0 root         (0) root         (0)     5365 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/workspace/config_schema/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     6130 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/workspace/config_schema/kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:00.934475 dagster_cloud-1.3.6/dagster_cloud/workspace/docker/
+-rw-r--r--   0 root         (0) root         (0)    12011 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/workspace/docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      327 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/workspace/docker/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:00.938475 dagster_cloud-1.3.6/dagster_cloud/workspace/ecs/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/workspace/ecs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23300 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/workspace/ecs/client.py
+-rw-r--r--   0 root         (0) root         (0)    22551 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/workspace/ecs/launcher.py
+-rw-r--r--   0 root         (0) root         (0)      694 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/workspace/ecs/run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     4165 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/workspace/ecs/service.py
+-rw-r--r--   0 root         (0) root         (0)     1748 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/workspace/ecs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:00.942475 dagster_cloud-1.3.6/dagster_cloud/workspace/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/workspace/kubernetes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17127 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/workspace/kubernetes/launcher.py
+-rw-r--r--   0 root         (0) root         (0)    11407 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/workspace/kubernetes/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1268 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/workspace/origin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:00.946475 dagster_cloud-1.3.6/dagster_cloud/workspace/user_code_launcher/
+-rw-r--r--   0 root         (0) root         (0)      745 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/workspace/user_code_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12807 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/workspace/user_code_launcher/process.py
+-rw-r--r--   0 root         (0) root         (0)    74026 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1209 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/dagster_cloud/workspace/user_code_launcher/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:00.886475 dagster_cloud-1.3.6/dagster_cloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4537 2023-05-25 17:28:00.000000 dagster_cloud-1.3.6/dagster_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3216 2023-05-25 17:28:00.000000 dagster_cloud-1.3.6/dagster_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 17:28:00.000000 dagster_cloud-1.3.6/dagster_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-25 17:28:00.000000 dagster_cloud-1.3.6/dagster_cloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-25 17:28:00.000000 dagster_cloud-1.3.6/dagster_cloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 17:28:00.946475 dagster_cloud-1.3.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2890 2023-05-25 17:17:05.000000 dagster_cloud-1.3.6/setup.py
```

### Comparing `dagster_cloud-1.3.5/PKG-INFO` & `dagster_cloud-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster_cloud
-Version: 1.3.5
+Version: 1.3.6
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
```

### Comparing `dagster_cloud-1.3.5/README.md` & `dagster_cloud-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/agent/cli/__init__.py` & `dagster_cloud-1.3.6/dagster_cloud/agent/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/agent/dagster_cloud_agent.py` & `dagster_cloud-1.3.6/dagster_cloud/agent/dagster_cloud_agent.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/agent/queries.py` & `dagster_cloud-1.3.6/dagster_cloud/agent/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/api/dagster_cloud_api.py` & `dagster_cloud-1.3.6/dagster_cloud/api/dagster_cloud_api.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/auth/constants.py` & `dagster_cloud-1.3.6/dagster_cloud/auth/constants.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/execution/cloud_run_launcher/process.py` & `dagster_cloud-1.3.6/dagster_cloud/execution/cloud_run_launcher/process.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/execution/monitoring/__init__.py` & `dagster_cloud-1.3.6/dagster_cloud/execution/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/execution/utils/process.py` & `dagster_cloud-1.3.6/dagster_cloud/execution/utils/process.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/instance/__init__.py` & `dagster_cloud-1.3.6/dagster_cloud/instance/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py` & `dagster_cloud-1.3.6/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py` & `dagster_cloud-1.3.6/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/pex/grpc/client.py` & `dagster_cloud-1.3.6/dagster_cloud/pex/grpc/client.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/pex/grpc/compile.py` & `dagster_cloud-1.3.6/dagster_cloud/pex/grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/pex/grpc/server/cli/__init__.py` & `dagster_cloud-1.3.6/dagster_cloud/pex/grpc/server/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/pex/grpc/server/manager.py` & `dagster_cloud-1.3.6/dagster_cloud/pex/grpc/server/manager.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/pex/grpc/server/registry.py` & `dagster_cloud-1.3.6/dagster_cloud/pex/grpc/server/registry.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/pex/grpc/server/server.py` & `dagster_cloud-1.3.6/dagster_cloud/pex/grpc/server/server.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/pex/grpc/types.py` & `dagster_cloud-1.3.6/dagster_cloud/pex/grpc/types.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/secrets/loader.py` & `dagster_cloud-1.3.6/dagster_cloud/secrets/loader.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/serverless/io_manager.py` & `dagster_cloud-1.3.6/dagster_cloud/serverless/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/storage/client.py` & `dagster_cloud-1.3.6/dagster_cloud/storage/client.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/storage/compute_logs/compute_log_manager.py` & `dagster_cloud-1.3.6/dagster_cloud/storage/compute_logs/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/storage/event_logs/queries.py` & `dagster_cloud-1.3.6/dagster_cloud/storage/event_logs/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/storage/event_logs/storage.py` & `dagster_cloud-1.3.6/dagster_cloud/storage/event_logs/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,14 +183,15 @@
                 {"key": tag_key},
                 ({"value": tag_value} if isinstance(tag_value, str) else {"values": tag_value}),
             )
             for tag_key, tag_value in event_records_filter.tags.items()
         ]
         if event_records_filter.tags
         else None,
+        "storageIds": event_records_filter.storage_ids,
     }
 
 
 def _event_record_from_graphql(graphene_event_record: Dict) -> EventLogRecord:
     check.dict_param(graphene_event_record, "graphene_event_record")
 
     return EventLogRecord(
```

### Comparing `dagster_cloud-1.3.5/dagster_cloud/storage/event_logs/utils.py` & `dagster_cloud-1.3.6/dagster_cloud/storage/event_logs/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/storage/runs/queries.py` & `dagster_cloud-1.3.6/dagster_cloud/storage/runs/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/storage/runs/storage.py` & `dagster_cloud-1.3.6/dagster_cloud/storage/runs/storage.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/storage/schedules/queries.py` & `dagster_cloud-1.3.6/dagster_cloud/storage/schedules/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/storage/schedules/storage.py` & `dagster_cloud-1.3.6/dagster_cloud/storage/schedules/storage.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/util/__init__.py` & `dagster_cloud-1.3.6/dagster_cloud/util/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/workspace/cli/__init__.py` & `dagster_cloud-1.3.6/dagster_cloud/workspace/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/workspace/config_schema/__init__.py` & `dagster_cloud-1.3.6/dagster_cloud/workspace/config_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/workspace/config_schema/docker.py` & `dagster_cloud-1.3.6/dagster_cloud/workspace/config_schema/docker.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/workspace/config_schema/ecs.py` & `dagster_cloud-1.3.6/dagster_cloud/workspace/config_schema/ecs.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,14 +86,24 @@
         is_required=False,
         description=(
             "Mount points for data volumes in the main container of the task."
             " See https://docs.aws.amazon.com/AmazonECS/latest/developerguide/efs-volumes.html"
             " for more information."
         ),
     ),
+    "server_sidecar_containers": Field(
+        Array(Permissive({})),
+        is_required=False,
+        description="Additional sidecar containers to include in code server task definitions.",
+    ),
+    "run_sidecar_containers": Field(
+        Array(Permissive({})),
+        is_required=False,
+        description="Additional sidecar containers to include in run task definitions.",
+    ),
 }
 
 
 ECS_CONTAINER_CONTEXT_CONFIG = {
     "secrets": Field(
         Noneable(Array(Shape({"name": StringSource, "valueFrom": StringSource}))),
         is_required=False,
```

### Comparing `dagster_cloud-1.3.5/dagster_cloud/workspace/config_schema/kubernetes.py` & `dagster_cloud-1.3.6/dagster_cloud/workspace/config_schema/kubernetes.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/workspace/docker/__init__.py` & `dagster_cloud-1.3.6/dagster_cloud/workspace/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/workspace/ecs/client.py` & `dagster_cloud-1.3.6/dagster_cloud/workspace/ecs/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -407,14 +407,15 @@
         params = dict(
             cluster=self.cluster_name,
             serviceName=service_name,
             taskDefinition=task_definition_arn,
             launchType=self.launch_type,
             desiredCount=1,
             enableExecuteCommand=allow_ecs_exec,
+            propagateTags="SERVICE",
         )
         params["networkConfiguration"] = self.network_configuration
 
         if service_registry_arn:
             params["serviceRegistries"] = [{"registryArn": service_registry_arn}]
 
         if tags and self.taggable:
```

### Comparing `dagster_cloud-1.3.5/dagster_cloud/workspace/ecs/launcher.py` & `dagster_cloud-1.3.6/dagster_cloud/workspace/ecs/launcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,14 +60,16 @@
         ecs_grace_period=None,
         launch_type: Optional[str] = None,
         server_resources: Optional[Mapping[str, Any]] = None,
         run_resources: Optional[Mapping[str, Any]] = None,
         runtime_platform: Optional[Mapping[str, Any]] = None,
         mount_points: Optional[Sequence[Mapping[str, Any]]] = None,
         volumes: Optional[Sequence[Mapping[str, Any]]] = None,
+        server_sidecar_containers: Optional[Sequence[Mapping[str, Any]]] = None,
+        run_sidecar_containers: Optional[Sequence[Mapping[str, Any]]] = None,
         **kwargs,
     ):
         self.ecs = boto3.client("ecs")
         self.logs = boto3.client("logs")
         self.service_discovery = boto3.client("servicediscovery")
         self.secrets_manager = boto3.client("secretsmanager")
 
@@ -110,14 +112,21 @@
         self.run_resources = check.opt_mapping_param(run_resources, "run_resources")
 
         self.runtime_platform = check.opt_mapping_param(runtime_platform, "runtime_platform")
 
         self.mount_points = check.opt_sequence_param(mount_points, "mount_points")
         self.volumes = check.opt_sequence_param(volumes, "volumes")
 
+        self.server_sidecar_containers = check.opt_sequence_param(
+            server_sidecar_containers, "server_sidecar_containers"
+        )
+        self.run_sidecar_containers = check.opt_sequence_param(
+            run_sidecar_containers, "run_sidecar_containers"
+        )
+
         self.client = Client(
             cluster_name=self.cluster,
             subnet_ids=self.subnets,
             security_group_ids=security_group_ids,
             service_discovery_namespace_id=self.service_discovery_namespace_id,
             log_group=self.log_group,
             show_debug_cluster_info=self.show_debug_cluster_info,
@@ -238,16 +247,18 @@
         # reconciliation - this is used to indicate that we're ready to
         # serve requests
         Path("/opt/finished_initial_reconciliation_sentinel.txt").touch(exist_ok=True)
         self._logger.info(
             "Wrote liveness sentinel: indicating that agent is ready to serve requests"
         )
 
-    def _get_grpc_server_sidecars(self) -> Optional[List[Dict[str, Any]]]:
-        return None
+    def _get_grpc_server_sidecars(
+        self, container_context: EcsContainerContext
+    ) -> Optional[Sequence[Mapping[str, Any]]]:
+        return container_context.server_sidecar_containers
 
     def _get_service_cpu_override(self, container_context: EcsContainerContext) -> Optional[str]:
         return container_context.server_resources.get("cpu")
 
     def _get_service_memory_override(self, container_context: EcsContainerContext) -> Optional[str]:
         return container_context.server_resources.get("memory")
 
@@ -258,14 +269,25 @@
 
     def _get_enable_ecs_exec(self) -> bool:
         return False
 
     def _get_additional_grpc_server_env(self) -> Dict[str, str]:
         return {}
 
+    def _get_dagster_tags(self, deployment_name: str, location_name: str) -> Dict[str, str]:
+        return {
+            "dagster/deployment_name": get_ecs_human_readable_label(deployment_name),
+            "dagster/location_name": get_ecs_human_readable_label(
+                location_name,
+            ),
+            "dagster/location_hash": deterministic_label_for_location(
+                deployment_name, location_name
+            ),
+        }
+
     def _start_new_server_spinup(
         self, deployment_name: str, location_name: str, metadata: CodeDeploymentMetadata
     ) -> DagsterCloudGrpcServer:
         if metadata.pex_metadata:
             command = metadata.get_multipex_server_command(PORT)
             additional_env = metadata.get_multipex_server_env()
             tags = {
@@ -287,14 +309,16 @@
             server_resources=self.server_resources,
             run_resources=self.run_resources,
             task_role_arn=self.task_role_arn,
             execution_role_arn=self.execution_role_arn,
             runtime_platform=self.runtime_platform,
             mount_points=self.mount_points,
             volumes=self.volumes,
+            server_sidecar_containers=self.server_sidecar_containers,
+            run_sidecar_containers=self.run_sidecar_containers,
         ).merge(EcsContainerContext.create_from_config(metadata.container_context))
 
         environment = merge_dicts(
             container_context.get_environment_dict(),
             additional_env,
             self._get_additional_grpc_server_env(),
         )
@@ -310,26 +334,20 @@
             family=family,
             image=metadata.image,
             container_name=CONTAINER_NAME,
             command=command,
             execution_role_arn=container_context.execution_role_arn,
             env=environment,
             tags={
-                "dagster/deployment_name": get_ecs_human_readable_label(deployment_name),
-                "dagster/location_name": get_ecs_human_readable_label(
-                    location_name,
-                ),
-                "dagster/location_hash": deterministic_label_for_location(
-                    deployment_name, location_name
-                ),
+                **self._get_dagster_tags(deployment_name, location_name),
                 **tags,
             },
             task_role_arn=container_context.task_role_arn,
             secrets=container_context.get_secrets_dict(self.secrets_manager),
-            sidecars=self._get_grpc_server_sidecars(),
+            sidecars=self._get_grpc_server_sidecars(container_context),
             logger=self._logger,
             cpu=self._get_service_cpu_override(container_context),
             memory=self._get_service_memory_override(container_context),
             ephemeral_storage=self._get_service_ephemeral_storage_override(container_context),
             allow_ecs_exec=self._get_enable_ecs_exec(),
             runtime_platform=container_context.runtime_platform,
             mount_points=container_context.mount_points,
@@ -471,23 +489,25 @@
         ]
 
     def get_agent_id_for_server(self, handle: EcsServerHandleType) -> Optional[str]:
         # Need to get container for server handle, then get the agent tag from that.
         return handle.tags.get("dagster/agent_id")
 
     def _run_launcher_kwargs(self) -> Dict[str, Any]:
-        sidecars = self._get_grpc_server_sidecars()
-
         return dict(
             task_definition={
                 "log_group": self.log_group,
                 "execution_role_arn": self.execution_role_arn,
                 "requires_compatibilities": [self.launch_type],
                 **({"task_role_arn": self.task_role_arn} if self.task_role_arn else {}),
-                **({"sidecars": sidecars} if sidecars else {}),
+                **(
+                    {"sidecar_containers": self.run_sidecar_containers}
+                    if self.run_sidecar_containers
+                    else {}
+                ),
                 **({"runtime_platform": self.runtime_platform} if self.runtime_platform else {}),
                 **({"mount_points": self.mount_points} if self.mount_points else {}),
                 **({"volumes": self.volumes} if self.volumes else {}),
             },
             secrets=self.secrets,
             secrets_tag=self.secrets_tag,
             env_vars=self.env_vars,
```

### Comparing `dagster_cloud-1.3.5/dagster_cloud/workspace/ecs/run_launcher.py` & `dagster_cloud-1.3.6/dagster_cloud/workspace/ecs/run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/workspace/ecs/service.py` & `dagster_cloud-1.3.6/dagster_cloud/workspace/ecs/service.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/workspace/ecs/utils.py` & `dagster_cloud-1.3.6/dagster_cloud/workspace/ecs/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/workspace/kubernetes/launcher.py` & `dagster_cloud-1.3.6/dagster_cloud/workspace/kubernetes/launcher.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/workspace/kubernetes/utils.py` & `dagster_cloud-1.3.6/dagster_cloud/workspace/kubernetes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/workspace/origin.py` & `dagster_cloud-1.3.6/dagster_cloud/workspace/origin.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/workspace/user_code_launcher/__init__.py` & `dagster_cloud-1.3.6/dagster_cloud/workspace/user_code_launcher/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/workspace/user_code_launcher/process.py` & `dagster_cloud-1.3.6/dagster_cloud/workspace/user_code_launcher/process.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py` & `dagster_cloud-1.3.6/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/dagster_cloud/workspace/user_code_launcher/utils.py` & `dagster_cloud-1.3.6/dagster_cloud/workspace/user_code_launcher/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 def get_human_readable_label(name, length_limit, sanitize_fn):
     truncated_name = name[:length_limit]
     return sanitize_fn(truncated_name) if sanitize_fn else truncated_name
 
 
-def deterministic_label_for_location(deployment_name, location_name):
+def deterministic_label_for_location(deployment_name: str, location_name: str) -> str:
     """Need a label here that is a unique function of location name since we use it to
     search for existing deployments on update and remove them. Does not need to be human-readable.
     """
     m = hashlib.sha1()  # Creates a 40-byte hash
     m.update(f"{deployment_name}-{location_name}".encode("utf-8"))
 
     unique_label = m.hexdigest()
```

### Comparing `dagster_cloud-1.3.5/dagster_cloud.egg-info/PKG-INFO` & `dagster_cloud-1.3.6/dagster_cloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-cloud
-Version: 1.3.5
+Version: 1.3.6
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
```

### Comparing `dagster_cloud-1.3.5/dagster_cloud.egg-info/SOURCES.txt` & `dagster_cloud-1.3.6/dagster_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.5/setup.py` & `dagster_cloud-1.3.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,16 +36,16 @@
         "Slack": "https://dagster.io/slack",
         "Blog": "https://dagster.io/blog",
         "Newsletter": "https://dagster.io/newsletter-signup",
     },
     packages=find_packages(exclude=["dagster_cloud_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.3.5",
-        "dagster-cloud-cli==1.3.5",
+        "dagster==1.3.6",
+        "dagster-cloud-cli==1.3.6",
         "pex",
         "questionary",
         "requests",
         "typer[all]",
     ],
     extras_require={
         "tests": [
@@ -58,19 +58,19 @@
             "mypy",
             "paramiko",
             "pylint",
             "pytest",
             "types-PyYAML",
             "types-requests",
             "dagster-cloud-test-infra",
-            "dagster_k8s==0.19.5",
+            "dagster_k8s==0.19.6",
         ],
-        "docker": ["docker", "dagster_docker==0.19.5"],
-        "kubernetes": ["kubernetes", "dagster_k8s==0.19.5"],
-        "ecs": ["dagster_aws==0.19.5", "boto3"],
+        "docker": ["docker", "dagster_docker==0.19.6"],
+        "kubernetes": ["kubernetes", "dagster_k8s==0.19.6"],
+        "ecs": ["dagster_aws==0.19.6", "boto3"],
         "sandbox": ["supervisor"],
         "pex": ["boto3"],
         "serverless": ["boto3"],
     },
     author="Elementl",
     license="Apache-2.0",
     classifiers=[
```

