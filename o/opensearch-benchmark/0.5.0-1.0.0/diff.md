# Comparing `tmp/opensearch-benchmark-0.5.0.tar.gz` & `tmp/opensearch-benchmark-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensearch-benchmark-0.5.0.tar", last modified: Thu May 18 21:29:21 2023, max compression
+gzip compressed data, was "opensearch-benchmark-1.0.0.tar", last modified: Thu May 25 20:49:19 2023, max compression
```

## Comparing `opensearch-benchmark-0.5.0.tar` & `opensearch-benchmark-1.0.0.tar`

### file list

```diff
@@ -1,314 +1,314 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.135290 opensearch-benchmark-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-05-18 21:29:21.135290 opensearch-benchmark-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.111289 opensearch-benchmark-0.5.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.111289 opensearch-benchmark-0.5.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/docs/api/client-options.md
--rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/docs/api/execute-test.md
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/docs/api/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/docs/api/kill-running-process.md
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/docs/api/pipeline.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/docs/api/target-hosts.md
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/docs/api/test-mode.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/docs/api/workload.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/docs/get-started.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.111289 opensearch-benchmark-0.5.0/docs/user-guides/
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/docs/user-guides/create-pipeline.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/docs/user-guides/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.111289 opensearch-benchmark-0.5.0/opensearch_benchmark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-05-18 21:29:21.000000 opensearch-benchmark-0.5.0/opensearch_benchmark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-05-18 21:29:21.000000 opensearch-benchmark-0.5.0/opensearch_benchmark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 21:29:21.000000 opensearch-benchmark-0.5.0/opensearch_benchmark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-18 21:29:21.000000 opensearch-benchmark-0.5.0/opensearch_benchmark.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 21:29:20.000000 opensearch-benchmark-0.5.0/opensearch_benchmark.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-18 21:29:21.000000 opensearch-benchmark-0.5.0/opensearch_benchmark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-18 21:29:21.000000 opensearch-benchmark-0.5.0/opensearch_benchmark.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.115289 opensearch-benchmark-0.5.0/osbenchmark/
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/async_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    50515 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/benchmarkd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.115289 opensearch-benchmark-0.5.0/osbenchmark/builder/
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31285 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/cluster_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.115289 opensearch-benchmark-0.5.0/osbenchmark/builder/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.115289 opensearch-benchmark-0.5.0/osbenchmark/builder/configs/listers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/configs/listers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/configs/listers/plugin_config_instance_lister.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.115289 opensearch-benchmark-0.5.0/osbenchmark/builder/configs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/configs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/configs/utils/config_path_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.119289 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.119289 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/builders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/builders/binary_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/builders/source_binary_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/core_plugin_source_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/external_plugin_source_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/opensearch_distribution_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/opensearch_source_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/plugin_distribution_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.119289 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/repositories/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/repositories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/repositories/opensearch_distribution_repository_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/repositories/plugin_distribution_repository_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/repositories/repository_url_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/repositories/source_repository_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.119289 opensearch-benchmark-0.5.0/osbenchmark/builder/executors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/executors/exception_handling_shell_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/executors/local_shell_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/executors/shell_executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.119289 opensearch-benchmark-0.5.0/osbenchmark/builder/installers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/installers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/installers/bare_installer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/installers/docker_installer.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/installers/exception_handling_installer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/installers/installer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.119289 opensearch-benchmark-0.5.0/osbenchmark/builder/installers/preparers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/installers/preparers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/installers/preparers/opensearch_preparer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/installers/preparers/plugin_preparer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/installers/preparers/preparer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/java_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.119289 opensearch-benchmark-0.5.0/osbenchmark/builder/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/launchers/docker_launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/launchers/exception_handling_launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/launchers/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/launchers/local_process_launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/launchers/no_op_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.123289 opensearch-benchmark-0.5.0/osbenchmark/builder/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/models/architecture_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/models/bootstrap_phase.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/models/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/models/cluster_flavors.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/models/cluster_infra_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/models/config_instance_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/models/host.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/models/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/models/plugin_config_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/models/provision_config_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/models/provision_config_instance_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/models/provision_config_instance_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    24300 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/provision_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    23247 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/provisioner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.123289 opensearch-benchmark-0.5.0/osbenchmark/builder/provisioners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/provisioners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/provisioners/provisioner.py
--rw-r--r--   0 runner    (1001) docker     (123)    34133 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/supplier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.123289 opensearch-benchmark-0.5.0/osbenchmark/builder/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/utils/artifact_variables_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/utils/binary_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/utils/config_applier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/utils/git_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/utils/host_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/utils/java_home_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/utils/jdk_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/utils/path_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/builder/utils/template_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    77539 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/chart_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14714 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12970 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    88571 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/min-os-version.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.123289 opensearch-benchmark-0.5.0/osbenchmark/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/base-workload.json.j2
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/benchmark.ini
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/custom-query-workload.json.j2
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/default-query-workload.json.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/docker-compose.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/logging.json
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/metrics-template.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.123289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/core-plugins.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.123289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.123289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.123289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.123289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/default/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/default/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.123289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/default/templates/config/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/default/templates/config/opensearch.yml
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/http.ini
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/transport.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.127289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/16gheap.ini
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/1gheap.ini
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/24gheap.ini
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/2gheap.ini
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/4gheap.ini
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/8gheap.ini
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/basic-license.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/dbg_non_safepoints/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/dbg_non_safepoints/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.127289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/dbg_non_safepoints/templates/config/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/dbg_non_safepoints/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/debug-non-safepoints.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.127289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/config.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.127289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/templates/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/templates/config/opensearch.yml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/defaults.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.127289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea/templates/config/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.127289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp/templates/config/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp.ini
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/g1gc.ini
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/trial-license.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.127289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled/templates/config/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.127289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/config.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.127289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (123)    11731 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/log4j2.properties
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/opensearch.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.127289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/core-plugins.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.127289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.127289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.127289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.127289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/default/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/default/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.127289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/default/templates/config/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/default/templates/config/opensearch.yml
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/http.ini
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/transport.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.131290 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/16gheap.ini
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/1gheap.ini
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/24gheap.ini
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/2gheap.ini
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/4gheap.ini
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/8gheap.ini
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/basic-license.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/dbg_non_safepoints/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/dbg_non_safepoints/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.131290 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/dbg_non_safepoints/templates/config/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/dbg_non_safepoints/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/debug-non-safepoints.ini
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/defaults.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.107289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.131290 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea/templates/config/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.111289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.111289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.131290 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp/templates/config/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp.ini
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/g1gc.ini
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/parallelgc.ini
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/trial-license.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.111289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.111289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.131290 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled/templates/config/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.131290 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/config.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.111289 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.131290 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/jvm.options
--rw-r--r--   0 runner    (1001) docker     (123)    11321 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/log4j2.properties
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/opensearch.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/results-template.json
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/test-executions-template.json
--rw-r--r--   0 runner    (1001) docker     (123)    23167 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/resources/workload-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    34843 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/results_publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)    76561 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)    18757 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/test_execution_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.131290 opensearch-benchmark-0.5.0/osbenchmark/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/utils/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/utils/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (123)    20252 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7537 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/utils/jvm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/utils/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    12386 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/utils/net.py
--rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/utils/opts.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/utils/periodic_waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/utils/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/utils/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/utils/sysstats.py
--rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/utils/versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.135290 opensearch-benchmark-0.5.0/osbenchmark/worker_coordinator/
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/worker_coordinator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    89687 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/worker_coordinator/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/worker_coordinator/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    97801 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/worker_coordinator/worker_coordinator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.135290 opensearch-benchmark-0.5.0/osbenchmark/workload/
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/workload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79356 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/workload/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    55903 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/workload/params.py
--rw-r--r--   0 runner    (1001) docker     (123)    37160 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/workload/workload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.135290 opensearch-benchmark-0.5.0/osbenchmark/workload_generator/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/workload_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/workload_generator/corpus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/workload_generator/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/osbenchmark/workload_generator/workload_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.135290 opensearch-benchmark-0.5.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10512 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/scripts/expand-data-corpus.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-18 21:29:21.135290 opensearch-benchmark-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:29:21.135290 opensearch-benchmark-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/tests/test_async_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/tests/test_execution_orchestrator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 21:27:48.000000 opensearch-benchmark-0.5.0/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.572327 opensearch-benchmark-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-05-25 20:49:19.572327 opensearch-benchmark-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.536326 opensearch-benchmark-1.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.536326 opensearch-benchmark-1.0.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/docs/api/client-options.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/docs/api/execute-test.md
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/docs/api/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/docs/api/kill-running-process.md
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/docs/api/pipeline.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/docs/api/target-hosts.md
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/docs/api/test-mode.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/docs/api/workload.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/docs/get-started.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.536326 opensearch-benchmark-1.0.0/docs/user-guides/
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/docs/user-guides/create-pipeline.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/docs/user-guides/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.540326 opensearch-benchmark-1.0.0/opensearch_benchmark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-05-25 20:49:19.000000 opensearch-benchmark-1.0.0/opensearch_benchmark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-05-25 20:49:19.000000 opensearch-benchmark-1.0.0/opensearch_benchmark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 20:49:19.000000 opensearch-benchmark-1.0.0/opensearch_benchmark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-25 20:49:19.000000 opensearch-benchmark-1.0.0/opensearch_benchmark.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 20:49:19.000000 opensearch-benchmark-1.0.0/opensearch_benchmark.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-25 20:49:19.000000 opensearch-benchmark-1.0.0/opensearch_benchmark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 20:49:19.000000 opensearch-benchmark-1.0.0/opensearch_benchmark.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.540326 opensearch-benchmark-1.0.0/osbenchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/async_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50515 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/benchmarkd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.544326 opensearch-benchmark-1.0.0/osbenchmark/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31285 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/cluster_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.544326 opensearch-benchmark-1.0.0/osbenchmark/builder/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.544326 opensearch-benchmark-1.0.0/osbenchmark/builder/configs/listers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/configs/listers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/configs/listers/plugin_config_instance_lister.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.544326 opensearch-benchmark-1.0.0/osbenchmark/builder/configs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/configs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/configs/utils/config_path_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.544326 opensearch-benchmark-1.0.0/osbenchmark/builder/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/downloaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.544326 opensearch-benchmark-1.0.0/osbenchmark/builder/downloaders/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/downloaders/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/downloaders/builders/binary_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/downloaders/builders/source_binary_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/downloaders/core_plugin_source_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/downloaders/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/downloaders/external_plugin_source_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/downloaders/opensearch_distribution_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/downloaders/opensearch_source_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/downloaders/plugin_distribution_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.544326 opensearch-benchmark-1.0.0/osbenchmark/builder/downloaders/repositories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/downloaders/repositories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/downloaders/repositories/opensearch_distribution_repository_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/downloaders/repositories/plugin_distribution_repository_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/downloaders/repositories/repository_url_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/downloaders/repositories/source_repository_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.544326 opensearch-benchmark-1.0.0/osbenchmark/builder/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/executors/exception_handling_shell_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/executors/local_shell_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/executors/shell_executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.548326 opensearch-benchmark-1.0.0/osbenchmark/builder/installers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/installers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/installers/bare_installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/installers/docker_installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/installers/exception_handling_installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/installers/installer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.548326 opensearch-benchmark-1.0.0/osbenchmark/builder/installers/preparers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/installers/preparers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/installers/preparers/opensearch_preparer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/installers/preparers/plugin_preparer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/installers/preparers/preparer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/java_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.548326 opensearch-benchmark-1.0.0/osbenchmark/builder/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/launchers/docker_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/launchers/exception_handling_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/launchers/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/launchers/local_process_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/launchers/no_op_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.548326 opensearch-benchmark-1.0.0/osbenchmark/builder/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/models/architecture_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/models/bootstrap_phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/models/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/models/cluster_flavors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/models/cluster_infra_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/models/config_instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/models/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/models/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/models/plugin_config_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/models/provision_config_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/models/provision_config_instance_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/models/provision_config_instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24300 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/provision_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23247 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/provisioner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.548326 opensearch-benchmark-1.0.0/osbenchmark/builder/provisioners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/provisioners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/provisioners/provisioner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34133 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/supplier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.552326 opensearch-benchmark-1.0.0/osbenchmark/builder/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/utils/artifact_variables_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/utils/binary_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/utils/config_applier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/utils/git_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/utils/host_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/utils/java_home_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/utils/jdk_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/utils/path_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/builder/utils/template_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77539 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/chart_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14714 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12970 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88962 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/min-os-version.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.552326 opensearch-benchmark-1.0.0/osbenchmark/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/base-workload.json.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/benchmark.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/custom-query-workload.json.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/default-query-workload.json.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/docker-compose.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/logging.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/metrics-template.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.532326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.532326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.532326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.552326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/core-plugins.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.556326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.556326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.556326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.556326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.532326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/default/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.532326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/default/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.556326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/default/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/default/templates/config/opensearch.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/http.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/transport_nio/transport.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.532326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.560326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/16gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/1gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/24gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/2gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/4gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/8gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/basic-license.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.532326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/dbg_non_safepoints/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.532326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/dbg_non_safepoints/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.560326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/dbg_non_safepoints/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/dbg_non_safepoints/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/debug-non-safepoints.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.560326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/config.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.532326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.560326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/templates/config/opensearch.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/defaults.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.532326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.532326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.560326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/ea.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.532326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.532326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.560326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/fp.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/g1gc.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/trial-license.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.532326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.532326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.560326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/unpooled.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.560326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/config.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.532326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.560326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (123)    11731 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/log4j2.properties
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/opensearch.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.536326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.532326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.560326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/plugins/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/plugins/v1/core-plugins.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.560326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.560326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.560326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.560326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.536326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/default/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.536326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/default/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.560326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/default/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/default/templates/config/opensearch.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/http.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/plugins/v1/transport_nio/transport.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.536326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.564326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/16gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/1gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/24gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/2gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/4gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/8gheap.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/basic-license.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.536326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/dbg_non_safepoints/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.536326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/dbg_non_safepoints/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.564326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/dbg_non_safepoints/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/dbg_non_safepoints/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/debug-non-safepoints.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/defaults.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.536326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.536326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.564326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/ea.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.536326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.536326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.564326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/fp.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/g1gc.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/parallelgc.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/trial-license.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.536326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.536326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.564326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/unpooled.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.568327 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/config.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.536326 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.568327 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/jvm.options
+-rw-r--r--   0 runner    (1001) docker     (123)    11321 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/log4j2.properties
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/opensearch.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/results-template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/test-executions-template.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23167 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/resources/workload-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34843 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/results_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76561 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18757 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/test_execution_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.568327 opensearch-benchmark-1.0.0/osbenchmark/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/utils/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/utils/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20252 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7537 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/utils/jvm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/utils/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12386 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/utils/net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/utils/opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/utils/periodic_waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/utils/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/utils/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/utils/sysstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/utils/versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.572327 opensearch-benchmark-1.0.0/osbenchmark/worker_coordinator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/worker_coordinator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89687 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/worker_coordinator/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/worker_coordinator/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97801 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/worker_coordinator/worker_coordinator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.572327 opensearch-benchmark-1.0.0/osbenchmark/workload/
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/workload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79356 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/workload/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55903 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/workload/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37160 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/workload/workload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.572327 opensearch-benchmark-1.0.0/osbenchmark/workload_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/workload_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/workload_generator/corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/workload_generator/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/osbenchmark/workload_generator/workload_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.572327 opensearch-benchmark-1.0.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10512 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/scripts/expand-data-corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-25 20:49:19.572327 opensearch-benchmark-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:49:19.572327 opensearch-benchmark-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/tests/test_async_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/tests/test_execution_orchestrator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 20:48:06.000000 opensearch-benchmark-1.0.0/version.txt
```

### Comparing `opensearch-benchmark-0.5.0/AUTHORS` & `opensearch-benchmark-1.0.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/CONTRIBUTING.md` & `opensearch-benchmark-1.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/LICENSE` & `opensearch-benchmark-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/PKG-INFO` & `opensearch-benchmark-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensearch-benchmark
-Version: 0.5.0
+Version: 1.0.0
 Summary: Macrobenchmarking framework for OpenSearch
 Home-page: https://github.com/opensearch-project/OpenSearch-Benchmark
 Maintainer: Ian Hoang, Govind Kamat
 Maintainer-email: hoangia@amazon.com, govkamat@amazon.com
 License: Apache License, Version 2.0
 Classifier: Topic :: System :: Benchmark
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `opensearch-benchmark-0.5.0/README.md` & `opensearch-benchmark-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/docs/api/execute-test.md` & `opensearch-benchmark-1.0.0/docs/api/execute-test.md`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/docs/user-guides/create-pipeline.md` & `opensearch-benchmark-1.0.0/docs/user-guides/create-pipeline.md`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/opensearch_benchmark.egg-info/PKG-INFO` & `opensearch-benchmark-1.0.0/opensearch_benchmark.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensearch-benchmark
-Version: 0.5.0
+Version: 1.0.0
 Summary: Macrobenchmarking framework for OpenSearch
 Home-page: https://github.com/opensearch-project/OpenSearch-Benchmark
 Maintainer: Ian Hoang, Govind Kamat
 Maintainer-email: hoangia@amazon.com, govkamat@amazon.com
 License: Apache License, Version 2.0
 Classifier: Topic :: System :: Benchmark
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `opensearch-benchmark-0.5.0/opensearch_benchmark.egg-info/SOURCES.txt` & `opensearch-benchmark-1.0.0/opensearch_benchmark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/__init__.py` & `opensearch-benchmark-1.0.0/osbenchmark/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/actor.py` & `opensearch-benchmark-1.0.0/osbenchmark/actor.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/async_connection.py` & `opensearch-benchmark-1.0.0/osbenchmark/async_connection.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/benchmark.py` & `opensearch-benchmark-1.0.0/osbenchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/benchmarkd.py` & `opensearch-benchmark-1.0.0/osbenchmark/benchmarkd.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/__init__.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/builder.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/builder.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/cluster.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/cluster.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/cluster_builder.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/cluster_builder.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/configs/listers/plugin_config_instance_lister.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/configs/listers/plugin_config_instance_lister.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/configs/utils/config_path_resolver.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/configs/utils/config_path_resolver.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/builders/binary_builder.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/downloaders/builders/binary_builder.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/builders/source_binary_builder.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/downloaders/builders/source_binary_builder.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/core_plugin_source_downloader.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/downloaders/core_plugin_source_downloader.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/downloader.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/downloaders/downloader.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/external_plugin_source_downloader.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/downloaders/external_plugin_source_downloader.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/opensearch_distribution_downloader.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/downloaders/opensearch_distribution_downloader.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/opensearch_source_downloader.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/downloaders/opensearch_source_downloader.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/plugin_distribution_downloader.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/downloaders/plugin_distribution_downloader.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/repositories/opensearch_distribution_repository_provider.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/downloaders/repositories/opensearch_distribution_repository_provider.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/repositories/plugin_distribution_repository_provider.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/downloaders/repositories/plugin_distribution_repository_provider.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/repositories/repository_url_provider.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/downloaders/repositories/repository_url_provider.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/downloaders/repositories/source_repository_provider.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/downloaders/repositories/source_repository_provider.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/executors/local_shell_executor.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/executors/local_shell_executor.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/executors/shell_executor.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/executors/shell_executor.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/installers/bare_installer.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/installers/bare_installer.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/installers/docker_installer.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/installers/docker_installer.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/installers/exception_handling_installer.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/installers/exception_handling_installer.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/installers/installer.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/installers/installer.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/installers/preparers/opensearch_preparer.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/installers/preparers/opensearch_preparer.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/installers/preparers/plugin_preparer.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/installers/preparers/plugin_preparer.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/installers/preparers/preparer.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/installers/preparers/preparer.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/java_resolver.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/java_resolver.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/launcher.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/launcher.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/launchers/docker_launcher.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/launchers/docker_launcher.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/launchers/exception_handling_launcher.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/launchers/exception_handling_launcher.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/launchers/launcher.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/launchers/launcher.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/launchers/local_process_launcher.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/launchers/local_process_launcher.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/models/architecture_types.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/models/architecture_types.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/models/config_instance_types.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/models/config_instance_types.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/models/plugin_config_instance.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/models/plugin_config_instance.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/models/provision_config_instance.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/models/provision_config_instance.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/models/provision_config_instance_descriptor.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/models/provision_config_instance_descriptor.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/provision_config.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/provision_config.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/provisioner.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/provisioner.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/provisioners/provisioner.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/provisioners/provisioner.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/supplier.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/supplier.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/utils/artifact_variables_provider.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/utils/artifact_variables_provider.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/utils/config_applier.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/utils/config_applier.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/utils/git_manager.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/utils/git_manager.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/utils/host_cleaner.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/utils/host_cleaner.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/utils/java_home_resolver.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/utils/java_home_resolver.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/utils/jdk_resolver.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/utils/jdk_resolver.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/utils/path_manager.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/utils/path_manager.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/builder/utils/template_renderer.py` & `opensearch-benchmark-1.0.0/osbenchmark/builder/utils/template_renderer.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/chart_generator.py` & `opensearch-benchmark-1.0.0/osbenchmark/chart_generator.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/client.py` & `opensearch-benchmark-1.0.0/osbenchmark/client.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/config.py` & `opensearch-benchmark-1.0.0/osbenchmark/config.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/exceptions.py` & `opensearch-benchmark-1.0.0/osbenchmark/exceptions.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/log.py` & `opensearch-benchmark-1.0.0/osbenchmark/log.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/metrics.py` & `opensearch-benchmark-1.0.0/osbenchmark/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,23 @@
 
     def __init__(self, cfg):
         self._config = cfg
         host = self._config.opts("results_publishing", "datastore.host")
         port = self._config.opts("results_publishing", "datastore.port")
         secure = convert.to_bool(self._config.opts("results_publishing", "datastore.secure"))
         user = self._config.opts("results_publishing", "datastore.user")
-        password = self._config.opts("results_publishing", "datastore.password")
+        try:
+            password = os.environ["OSB_DATASTORE_PASSWORD"]
+        except KeyError:
+            try:
+                password = self._config.opts("results_publishing", "datastore.password")
+            except exceptions.ConfigError:
+                raise exceptions.ConfigError(
+                    "No password configured through [results_publishing] configuration or OSB_DATASTORE_PASSWORD environment variable."
+                ) from None
         verify = self._config.opts("results_publishing", "datastore.ssl.verification_mode", default_value="full", mandatory=False) != "none"
         ca_path = self._config.opts("results_publishing", "datastore.ssl.certificate_authorities", default_value=None, mandatory=False)
         self.probe_version = self._config.opts("results_publishing", "datastore.probe.cluster_version", default_value=True, mandatory=False)
 
         # Instead of duplicating code, we're just adapting the metrics store specific properties to match the regular client options.
         client_options = {
             "use_ssl": secure,
@@ -1534,15 +1542,15 @@
         else:
             raise exceptions.NotFound("No test_execution with test_execution id [{}]".format(test_execution_id))
 
 
 class OsResultsStore:
     """
     Stores the results of a test_execution in a format that is
-    better suited for reporting with Kibana.
+    better suited for reporting with OpenSearch Dashboards.
     """
     INDEX_PREFIX = "benchmark-results-"
     RESULTS_DOC_TYPE = "_doc"
 
     def __init__(self, cfg, client_factory_class=OsClientFactory, index_template_provider_class=IndexTemplateProvider):
         """
         Creates a new results store.
```

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/paths.py` & `opensearch-benchmark-1.0.0/osbenchmark/paths.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/resources/base-workload.json.j2` & `opensearch-benchmark-1.0.0/osbenchmark/resources/base-workload.json.j2`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/resources/benchmark.ini` & `opensearch-benchmark-1.0.0/osbenchmark/resources/benchmark.ini`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/resources/docker-compose.yml.j2` & `opensearch-benchmark-1.0.0/osbenchmark/resources/docker-compose.yml.j2`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/resources/logging.json` & `opensearch-benchmark-1.0.0/osbenchmark/resources/logging.json`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/resources/metrics-template.json` & `opensearch-benchmark-1.0.0/osbenchmark/resources/metrics-template.json`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/core-plugins.txt` & `opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/core-plugins.txt`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/README.md` & `opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/README.md`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/plugin.py` & `opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_azure/plugin.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/README.md` & `opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/README.md`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/plugin.py` & `opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_gcs/plugin.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/README.md` & `opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/README.md`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/plugin.py` & `opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/plugins/v1/repository_s3/plugin.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/config.ini` & `opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/default_distro/config.ini`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/README.md` & `opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/README.md`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/config.ini` & `opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/config.ini`

 * *Files 9% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 jdk.bundled.release_url = https://artifacts.opensearch.org/releases/bundle/opensearch/{{VERSION}}/opensearch-{{VERSION}}-{{OSNAME}}-{{ARCH}}.tar.gz
 jdk.unbundled.release_url = https://artifacts.opensearch.org/releases/bundle/opensearch/{{VERSION}}/opensearch-{{VERSION}}-{{OSNAME}}-{{ARCH}}.tar.gz
 
 docker_image=opensearchproject/opensearch
 # major version of the JDK that is used to build OpenSearch
 build.jdk = 12
 # list of JDK major versions that are used to run OpenSearch
-runtime.jdk = 12,11,8
+runtime.jdk = 17,16,15,14,13,12,11,8
 runtime.jdk.bundled = true
```

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/jvm.options` & `opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/jvm.options`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/log4j2.properties` & `opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/log4j2.properties`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/opensearch.yml` & `opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/1.0/provision_config_instances/v1/vanilla/templates/config/opensearch.yml`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/core-plugins.txt` & `opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/plugins/v1/core-plugins.txt`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/README.md` & `opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/README.md`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/plugin.py` & `opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_azure/plugin.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/README.md` & `opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/README.md`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/plugin.py` & `opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_gcs/plugin.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/README.md` & `opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/README.md`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/plugin.py` & `opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/plugins/v1/repository_s3/plugin.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/README.md` & `opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/README.md`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/config.ini` & `opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/config.ini`

 * *Files 1% similar despite different names*

```diff
@@ -12,11 +12,11 @@
 release_url = https://artifacts.opensearch.org/releases/bundle/opensearch/{{VERSION}}/opensearch-{{VERSION}}-{{OSNAME}}-{{ARCH}}.tar.gz
 # new DISCLAIMER: OpenSearch already comes integrated with JDK
 jdk.bundled.release_url = https://artifacts.opensearch.org/releases/bundle/opensearch/{{VERSION}}/opensearch-{{VERSION}}-{{OSNAME}}-{{ARCH}}.tar.gz
 jdk.unbundled.release_url = https://artifacts.opensearch.org/releases/bundle/opensearch/{{VERSION}}/opensearch-{{VERSION}}-{{OSNAME}}-{{ARCH}}.tar.gz
 
 docker_image=opensearchproject/opensearch
 # major version of the JDK that is used to build OpenSearch
-build.jdk = 16
+build.jdk = 17
 # list of JDK major versions that are used to run OpenSearch
-runtime.jdk = 16,15,14,13,12,11
+runtime.jdk = 17,16,15,14,13,12,11,8
 runtime.jdk.bundled = true
```

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/jvm.options` & `opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/jvm.options`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/log4j2.properties` & `opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/log4j2.properties`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/opensearch.yml` & `opensearch-benchmark-1.0.0/osbenchmark/resources/provision_configs/main/provision_config_instances/v1/vanilla/templates/config/opensearch.yml`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/resources/results-template.json` & `opensearch-benchmark-1.0.0/osbenchmark/resources/results-template.json`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/resources/test-executions-template.json` & `opensearch-benchmark-1.0.0/osbenchmark/resources/test-executions-template.json`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/resources/workload-schema.json` & `opensearch-benchmark-1.0.0/osbenchmark/resources/workload-schema.json`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/results_publisher.py` & `opensearch-benchmark-1.0.0/osbenchmark/results_publisher.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/telemetry.py` & `opensearch-benchmark-1.0.0/osbenchmark/telemetry.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/test_execution_orchestrator.py` & `opensearch-benchmark-1.0.0/osbenchmark/test_execution_orchestrator.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/time.py` & `opensearch-benchmark-1.0.0/osbenchmark/time.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/utils/__init__.py` & `opensearch-benchmark-1.0.0/osbenchmark/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/utils/collections.py` & `opensearch-benchmark-1.0.0/osbenchmark/utils/collections.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/utils/console.py` & `opensearch-benchmark-1.0.0/osbenchmark/utils/console.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/utils/convert.py` & `opensearch-benchmark-1.0.0/osbenchmark/utils/convert.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/utils/git.py` & `opensearch-benchmark-1.0.0/osbenchmark/utils/git.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/utils/io.py` & `opensearch-benchmark-1.0.0/osbenchmark/utils/io.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/utils/jvm.py` & `opensearch-benchmark-1.0.0/osbenchmark/utils/jvm.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/utils/modules.py` & `opensearch-benchmark-1.0.0/osbenchmark/utils/modules.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/utils/net.py` & `opensearch-benchmark-1.0.0/osbenchmark/utils/net.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/utils/opts.py` & `opensearch-benchmark-1.0.0/osbenchmark/utils/opts.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/utils/periodic_waiter.py` & `opensearch-benchmark-1.0.0/osbenchmark/utils/periodic_waiter.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/utils/process.py` & `opensearch-benchmark-1.0.0/osbenchmark/utils/process.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/utils/repo.py` & `opensearch-benchmark-1.0.0/osbenchmark/utils/repo.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/utils/sysstats.py` & `opensearch-benchmark-1.0.0/osbenchmark/utils/sysstats.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/utils/versions.py` & `opensearch-benchmark-1.0.0/osbenchmark/utils/versions.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/version.py` & `opensearch-benchmark-1.0.0/osbenchmark/version.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/worker_coordinator/__init__.py` & `opensearch-benchmark-1.0.0/osbenchmark/worker_coordinator/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/worker_coordinator/runner.py` & `opensearch-benchmark-1.0.0/osbenchmark/worker_coordinator/runner.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/worker_coordinator/scheduler.py` & `opensearch-benchmark-1.0.0/osbenchmark/worker_coordinator/scheduler.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/worker_coordinator/worker_coordinator.py` & `opensearch-benchmark-1.0.0/osbenchmark/worker_coordinator/worker_coordinator.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/workload/__init__.py` & `opensearch-benchmark-1.0.0/osbenchmark/workload/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/workload/loader.py` & `opensearch-benchmark-1.0.0/osbenchmark/workload/loader.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/workload/params.py` & `opensearch-benchmark-1.0.0/osbenchmark/workload/params.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/workload/workload.py` & `opensearch-benchmark-1.0.0/osbenchmark/workload/workload.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/workload_generator/__init__.py` & `opensearch-benchmark-1.0.0/osbenchmark/workload_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/workload_generator/corpus.py` & `opensearch-benchmark-1.0.0/osbenchmark/workload_generator/corpus.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/workload_generator/index.py` & `opensearch-benchmark-1.0.0/osbenchmark/workload_generator/index.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/osbenchmark/workload_generator/workload_generator.py` & `opensearch-benchmark-1.0.0/osbenchmark/workload_generator/workload_generator.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/scripts/expand-data-corpus.py` & `opensearch-benchmark-1.0.0/scripts/expand-data-corpus.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/setup.py` & `opensearch-benchmark-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/tests/test_async_connection.py` & `opensearch-benchmark-1.0.0/tests/test_async_connection.py`

 * *Files identical despite different names*

### Comparing `opensearch-benchmark-0.5.0/tests/test_execution_orchestrator_test.py` & `opensearch-benchmark-1.0.0/tests/test_execution_orchestrator_test.py`

 * *Files identical despite different names*

