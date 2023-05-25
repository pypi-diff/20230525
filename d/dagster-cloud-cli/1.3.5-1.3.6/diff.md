# Comparing `tmp/dagster_cloud_cli-1.3.5.tar.gz` & `tmp/dagster_cloud_cli-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_cloud_cli-1.3.5.tar", last modified: Thu May 18 20:49:53 2023, max compression
+gzip compressed data, was "dagster_cloud_cli-1.3.6.tar", last modified: Thu May 25 17:28:06 2023, max compression
```

## Comparing `dagster_cloud_cli-1.3.5.tar` & `dagster_cloud_cli-1.3.6.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.285681 dagster_cloud_cli-1.3.5/
--rw-r--r--   0 root         (0) root         (0)      132 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      314 2023-05-18 20:49:53.285681 dagster_cloud_cli-1.3.5/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.249681 dagster_cloud_cli-1.3.5/dagster_cloud_cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.249681 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.249681 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/branch_deployment/
--rw-r--r--   0 root         (0) root         (0)     4612 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/branch_deployment/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.253681 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/ci/
--rw-r--r--   0 root         (0) root         (0)    24628 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/ci/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4124 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/ci/checks.py
--rw-r--r--   0 root         (0) root         (0)     1872 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/ci/report.py
--rw-r--r--   0 root         (0) root         (0)     4114 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/ci/state.py
--rw-r--r--   0 root         (0) root         (0)      508 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/ci/utils.py
--rw-r--r--   0 root         (0) root         (0)     8622 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.253681 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/deployment/
--rw-r--r--   0 root         (0) root         (0)     1508 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/deployment/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.257681 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/deployment/alert_policies/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/deployment/alert_policies/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1570 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/deployment/alert_policies/commands.py
--rw-r--r--   0 root         (0) root         (0)     5883 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.257681 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/job/
--rw-r--r--   0 root         (0) root         (0)     1926 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/job/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4233 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.257681 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/organization/
--rw-r--r--   0 root         (0) root         (0)     2129 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/organization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.257681 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/organization/saml/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/organization/saml/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2707 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/organization/saml/commands.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.261681 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/run/
--rw-r--r--   0 root         (0) root         (0)      669 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/run/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.261681 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/serverless/
--rw-r--r--   0 root         (0) root         (0)     1499 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/serverless/Dockerfile
--rw-r--r--   0 root         (0) root         (0)      628 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli
--rw-r--r--   0 root         (0) root         (0)    17755 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/serverless/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.261681 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/workspace/
--rw-r--r--   0 root         (0) root         (0)    11997 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18291 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/config_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.269681 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      424 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/_utils.py
--rw-r--r--   0 root         (0) root         (0)     1744 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/docker_runner.py
--rw-r--r--   0 root         (0) root         (0)     1122 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/errors.py
--rw-r--r--   0 root         (0) root         (0)     9228 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/graphql_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.269681 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/headers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/headers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      376 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/headers/auth.py
--rw-r--r--   0 root         (0) root         (0)      958 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/headers/impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.269681 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/headers/versioning/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/headers/versioning/__init__.py
--rw-r--r--   0 root         (0) root         (0)       96 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/headers/versioning/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.281681 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/
--rw-r--r--   0 root         (0) root         (0)      172 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1680 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/code_location.py
--rw-r--r--   0 root         (0) root         (0)     9467 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/deploy.py
--rw-r--r--   0 root         (0) root         (0)    13847 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/deps.py
--rw-r--r--   0 root         (0) root         (0)      949 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/git_context.py
--rw-r--r--   0 root         (0) root         (0)     6992 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/github_context.py
--rw-r--r--   0 root         (0) root         (0)     1063 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/gitlab_context.py
--rw-r--r--   0 root         (0) root         (0)     1232 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/parse_workspace.py
--rw-r--r--   0 root         (0) root         (0)     4655 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/pex_registry.py
--rw-r--r--   0 root         (0) root         (0)      709 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/selftest.py
--rw-r--r--   0 root         (0) root         (0)     4496 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/source.py
--rw-r--r--   0 root         (0) root         (0)     5913 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/util.py
--rw-r--r--   0 root         (0) root         (0)     1920 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pydantic_yaml.py
--rw-r--r--   0 root         (0) root         (0)     5384 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/workspace.py
--rw-r--r--   0 root         (0) root         (0)     2513 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/docker_utils.py
--rw-r--r--   0 root         (0) root         (0)     6700 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)    18577 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/gql.py
--rw-r--r--   0 root         (0) root         (0)     5859 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/pex_utils.py
--rw-r--r--   0 root         (0) root         (0)     1378 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/types.py
--rw-r--r--   0 root         (0) root         (0)     2804 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/ui.py
--rw-r--r--   0 root         (0) root         (0)     3488 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.249681 dagster_cloud_cli-1.3.5/dagster_cloud_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      314 2023-05-18 20:49:53.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2950 2023-05-18 20:49:53.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 20:49:53.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-05-18 20:49:53.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       97 2023-05-18 20:49:53.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-05-18 20:49:53.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:49:53.285681 dagster_cloud_cli-1.3.5/dagster_cloud_cli_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      189 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli_tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     3745 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli_tests/test_check.py
--rw-r--r--   0 root         (0) root         (0)    15513 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli_tests/test_ci_commands.py
--rw-r--r--   0 root         (0) root         (0)      659 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli_tests/test_gql.py
--rw-r--r--   0 root         (0) root         (0)     8767 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/dagster_cloud_cli_tests/test_metrics.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-18 20:49:53.285681 dagster_cloud_cli-1.3.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1101 2023-05-18 20:38:22.000000 dagster_cloud_cli-1.3.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:06.366502 dagster_cloud_cli-1.3.6/
+-rw-r--r--   0 root         (0) root         (0)      132 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      314 2023-05-25 17:28:06.366502 dagster_cloud_cli-1.3.6/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:06.334502 dagster_cloud_cli-1.3.6/dagster_cloud_cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:06.334502 dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:06.334502 dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/branch_deployment/
+-rw-r--r--   0 root         (0) root         (0)     4612 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/branch_deployment/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:06.338502 dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/ci/
+-rw-r--r--   0 root         (0) root         (0)    26608 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/ci/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4124 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/ci/checks.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/ci/report.py
+-rw-r--r--   0 root         (0) root         (0)     4114 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/ci/state.py
+-rw-r--r--   0 root         (0) root         (0)      508 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/ci/utils.py
+-rw-r--r--   0 root         (0) root         (0)     8622 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:06.338502 dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/deployment/
+-rw-r--r--   0 root         (0) root         (0)     1508 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/deployment/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:06.342502 dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/deployment/alert_policies/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/deployment/alert_policies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/deployment/alert_policies/commands.py
+-rw-r--r--   0 root         (0) root         (0)     5883 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:06.342502 dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/job/
+-rw-r--r--   0 root         (0) root         (0)     1926 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/job/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4233 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:06.342502 dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/organization/
+-rw-r--r--   0 root         (0) root         (0)     2129 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/organization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:06.342502 dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/organization/saml/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/organization/saml/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2707 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/organization/saml/commands.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:06.346502 dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/run/
+-rw-r--r--   0 root         (0) root         (0)      669 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/run/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:06.346502 dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/serverless/
+-rw-r--r--   0 root         (0) root         (0)     1499 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/serverless/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)      628 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli
+-rw-r--r--   0 root         (0) root         (0)    18121 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/serverless/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:06.346502 dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/workspace/
+-rw-r--r--   0 root         (0) root         (0)    11997 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18291 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/config_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:06.350502 dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      424 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1744 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/docker_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/errors.py
+-rw-r--r--   0 root         (0) root         (0)     9228 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/graphql_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:06.354502 dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/headers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/headers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      376 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/headers/auth.py
+-rw-r--r--   0 root         (0) root         (0)      958 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/headers/impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:06.354502 dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/headers/versioning/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/headers/versioning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       96 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/headers/versioning/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:06.362502 dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/pex_builder/
+-rw-r--r--   0 root         (0) root         (0)      172 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/pex_builder/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1680 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/pex_builder/code_location.py
+-rw-r--r--   0 root         (0) root         (0)     9467 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/pex_builder/deploy.py
+-rw-r--r--   0 root         (0) root         (0)    13847 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/pex_builder/deps.py
+-rw-r--r--   0 root         (0) root         (0)      949 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/pex_builder/git_context.py
+-rw-r--r--   0 root         (0) root         (0)     6992 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/pex_builder/github_context.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/pex_builder/gitlab_context.py
+-rw-r--r--   0 root         (0) root         (0)     1232 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/pex_builder/parse_workspace.py
+-rw-r--r--   0 root         (0) root         (0)     4655 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/pex_builder/pex_registry.py
+-rw-r--r--   0 root         (0) root         (0)      709 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/pex_builder/selftest.py
+-rw-r--r--   0 root         (0) root         (0)     4787 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/pex_builder/source.py
+-rw-r--r--   0 root         (0) root         (0)     5913 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/pex_builder/util.py
+-rw-r--r--   0 root         (0) root         (0)     1920 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/pydantic_yaml.py
+-rw-r--r--   0 root         (0) root         (0)     5384 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/workspace.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/docker_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6700 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)    18577 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/gql.py
+-rw-r--r--   0 root         (0) root         (0)     5859 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/pex_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/types.py
+-rw-r--r--   0 root         (0) root         (0)     2804 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/ui.py
+-rw-r--r--   0 root         (0) root         (0)     3488 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:06.334502 dagster_cloud_cli-1.3.6/dagster_cloud_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      314 2023-05-25 17:28:06.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2950 2023-05-25 17:28:06.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 17:28:06.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-05-25 17:28:06.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       97 2023-05-25 17:28:06.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-05-25 17:28:06.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:28:06.366502 dagster_cloud_cli-1.3.6/dagster_cloud_cli_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      189 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli_tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     3745 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli_tests/test_check.py
+-rw-r--r--   0 root         (0) root         (0)    16129 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli_tests/test_ci_commands.py
+-rw-r--r--   0 root         (0) root         (0)      659 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli_tests/test_gql.py
+-rw-r--r--   0 root         (0) root         (0)     8872 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/dagster_cloud_cli_tests/test_metrics.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 17:28:06.366502 dagster_cloud_cli-1.3.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1101 2023-05-25 17:17:05.000000 dagster_cloud_cli-1.3.6/setup.py
```

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/branch_deployment/__init__.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/branch_deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/ci/__init__.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/ci/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from dagster_cloud_cli.core.pex_builder import (
     code_location,
     deps,
     github_context,
     gitlab_context,
     parse_workspace,
 )
-from dagster_cloud_cli.types import CliEventTags
+from dagster_cloud_cli.types import CliEventTags, CliEventType
 
 
 @app.command(help="Print json information about current CI/CD environment")
 def inspect(project_dir: str):
     project_dir = os.path.abspath(project_dir)
     source = metrics.get_source()
     info = {"source": str(source), "project-dir": project_dir}
@@ -313,25 +313,25 @@
         else:
             ui.print(f"{location.location_name} DESELECTED")
 
 
 @app.command(help="Mark the specified locations as excluded from the current build session")
 def locations_deselect(
     location_names: List[str],
-    statedir: str = typer.Option(None, envvar="DAGSTER_BUILD_STATEDIR"),
+    statedir: str = STATEDIR_OPTION,
 ):
     state_store = state.FileStore(statedir=statedir)
     state_store.deselect(location_names)
     ui.print("Deselected locations: {locations_names}")
 
 
 @app.command(help="Mark the specified locations as included in the current build session")
 def locations_select(
     location_names: List[str],
-    statedir: str = typer.Option(None, envvar="DAGSTER_BUILD_STATEDIR"),
+    statedir: str = STATEDIR_OPTION,
 ):
     state_store = state.FileStore(statedir=statedir)
     state_store.select(location_names)
     ui.print("Deselected locations: {locations_names}")
 
 
 def _get_selected_locations(
@@ -352,15 +352,15 @@
 class BuildStrategy(Enum):
     pex = "python-executable"
     docker = "docker"
 
 
 @app.command(help="Build selected or requested locations")
 def build(
-    statedir: str = typer.Option(None, envvar="DAGSTER_BUILD_STATEDIR"),
+    statedir: str = STATEDIR_OPTION,
     location_name: List[str] = typer.Option([]),
     build_directory: Optional[str] = typer.Option(
         None,
         help=(
             "Directory root for building this code location. Read from dagster_cloud.yaml by"
             " default."
         ),
@@ -430,72 +430,42 @@
             elif (not build_directory) and configured_build_directory:
                 location_build_dir = configured_build_directory
             elif build_directory and (not configured_build_directory):
                 location_build_dir = build_directory
             else:
                 location_build_dir = "."
 
+            url = location_state.url
+            api_token = os.environ.get(TOKEN_ENV_VAR_NAME, "")
+
             if build_strategy == BuildStrategy.docker:
                 if not docker_base_image:
                     docker_base_image = f"python:{python_version}-slim"
-
-                ui.print(
-                    f"Building docker image for location {name} using base image"
-                    f" {docker_base_image}"
-                )
-                docker_utils.verify_docker()
-                registry_info = utils.get_registry_info(location_state.url)
-
-                docker_image_tag = docker_utils.default_image_tag(
-                    location_state.deployment_name, name, location_state.build.commit_hash
-                )
-
-                retval = docker_utils.build_image(
-                    location_build_dir,
-                    docker_image_tag,
-                    registry_info,
-                    env_vars=docker_env,
-                    base_image=docker_base_image,
+                location_state.build_output = _build_docker(
+                    url=url,
+                    api_token=api_token,
+                    name=name,
+                    location_build_dir=location_build_dir,
+                    docker_base_image=docker_base_image,
+                    docker_env=docker_env,
+                    location_state=location_state,
                 )
-                if retval != 0:
-                    raise ui.error(f"Failed to build docker image for location {name}")
-
-                retval = docker_utils.upload_image(docker_image_tag, registry_info)
-                if retval != 0:
-                    raise ui.error(f"Failed to upload docker image for location {name}")
-
-                image = f'{registry_info["registry_url"]}:{docker_image_tag}'
-
-                # Update and save build state
-                location_state.build_output = state.DockerBuildOutput(image=image)
                 state_store.save(location_state)
-                ui.print(f"Built and uploaded image {image} for location {name}")
             elif build_strategy == BuildStrategy.pex:
-                pex_location = parse_workspace.Location(
-                    name,
-                    directory=location_build_dir,
-                    build_folder=location_build_dir,
-                    location_file=location_state.location_file,
-                )
-                location_kwargs = pex_utils.build_upload_pex(
-                    url=location_state.url,
-                    api_token=os.environ[TOKEN_ENV_VAR_NAME],
-                    location=pex_location,
-                    build_method=pex_build_method,
-                    kwargs={
-                        "python_version": python_version,
-                        "base_image_tag": pex_base_image_tag,
-                        "deps_cache_from": pex_deps_cache_from,
-                        "deps_cache_to": pex_deps_cache_to,
-                    },
-                )
-                location_state.build_output = state.PexBuildOutput(
+                location_state.build_output = _build_pex(
+                    url=url,
+                    api_token=api_token,
+                    name=name,
+                    location_build_dir=location_build_dir,
                     python_version=python_version,
-                    image=location_kwargs["image"],
-                    pex_tag=location_kwargs["pex_tag"],
+                    pex_build_method=pex_build_method,
+                    pex_deps_cache_from=pex_deps_cache_from,
+                    pex_deps_cache_to=pex_deps_cache_to,
+                    pex_base_image_tag=pex_base_image_tag,
+                    location_state=location_state,
                 )
                 state_store.save(location_state)
                 ui.print(
                     "Built and uploaded python executable"
                     f" {location_state.build_output.pex_tag} for location {name}"
                 )
         except:
@@ -503,17 +473,103 @@
             state_store.save(location_state)
             raise
         else:
             location_state.add_status_change(state.LocationStatus.pending, "build successful")
             state_store.save(location_state)
 
 
+@metrics.instrument(
+    CliEventType.BUILD,
+    tags=[CliEventTags.subcommand.dagster_cloud_ci, CliEventTags.server_strategy.docker],
+)
+# url and api_token are used by the instrument decorator
+def _build_docker(
+    url: str,
+    api_token: str,
+    name: str,
+    location_build_dir: str,
+    docker_base_image: str,
+    docker_env: List[str],
+    location_state: state.LocationState,
+) -> state.DockerBuildOutput:
+    name = location_state.location_name
+    ui.print(f"Building docker image for location {name} using base image {docker_base_image}")
+    docker_utils.verify_docker()
+    registry_info = utils.get_registry_info(url)
+
+    docker_image_tag = docker_utils.default_image_tag(
+        location_state.deployment_name, name, location_state.build.commit_hash
+    )
+
+    retval = docker_utils.build_image(
+        location_build_dir,
+        docker_image_tag,
+        registry_info,
+        env_vars=docker_env,
+        base_image=docker_base_image,
+    )
+    if retval != 0:
+        raise ui.error(f"Failed to build docker image for location {name}")
+
+    retval = docker_utils.upload_image(docker_image_tag, registry_info)
+    if retval != 0:
+        raise ui.error(f"Failed to upload docker image for location {name}")
+
+    image = f'{registry_info["registry_url"]}:{docker_image_tag}'
+    ui.print(f"Built and uploaded image {image} for location {name}")
+
+    return state.DockerBuildOutput(image=image)
+
+
+@metrics.instrument(
+    CliEventType.BUILD,
+    tags=[CliEventTags.subcommand.dagster_cloud_ci, CliEventTags.server_strategy.pex],
+)
+# url and api_token are used by the instrument decorator
+def _build_pex(
+    url: str,
+    api_token: str,
+    name: str,
+    location_build_dir: str,
+    python_version: str,
+    pex_build_method: deps.BuildMethod,
+    pex_deps_cache_from: Optional[str],
+    pex_deps_cache_to: Optional[str],
+    pex_base_image_tag: Optional[str],
+    location_state: state.LocationState,
+) -> state.PexBuildOutput:
+    pex_location = parse_workspace.Location(
+        name,
+        directory=location_build_dir,
+        build_folder=location_build_dir,
+        location_file=location_state.location_file,
+    )
+
+    location_kwargs = pex_utils.build_upload_pex(
+        url=url,
+        api_token=api_token,
+        location=pex_location,
+        build_method=pex_build_method,
+        kwargs={
+            "python_version": python_version,
+            "base_image_tag": pex_base_image_tag,
+            "deps_cache_from": pex_deps_cache_from,
+            "deps_cache_to": pex_deps_cache_to,
+        },
+    )
+    return state.PexBuildOutput(
+        python_version=python_version,
+        image=location_kwargs["image"],
+        pex_tag=location_kwargs["pex_tag"],
+    )
+
+
 @app.command(help="Update the current build session for an externally built docker image.")
 def set_build_output(
-    statedir: str = typer.Option(None, envvar="DAGSTER_BUILD_STATEDIR"),
+    statedir: str = STATEDIR_OPTION,
     location_name: List[str] = typer.Option([]),
     image_tag: str = typer.Option(
         ...,
         help=(
             "Tag for the built docker image. Note the registry must be specified in"
             " dagster_cloud.yaml."
         ),
@@ -550,15 +606,15 @@
         state_store.save(location_state)
         ui.print(f"Recorded image {images[name]} for location {name}")
     ui.print("Use 'ci deploy' to update dagster-cloud.")
 
 
 @app.command(help="Deploy built code locations to dagster cloud.")
 def deploy(
-    statedir: str = typer.Option(None, envvar="DAGSTER_BUILD_STATEDIR"),
+    statedir: str = STATEDIR_OPTION,
     location_name: List[str] = typer.Option([]),
     location_load_timeout: int = LOCATION_LOAD_TIMEOUT_OPTION,
     agent_heartbeat_timeout: int = AGENT_HEARTBEAT_TIMEOUT_OPTION,
 ):
     state_store = state.FileStore(statedir=statedir)
     locations = _get_selected_locations(state_store, location_name)
     ui.print("Going deploy the following locations:")
@@ -578,48 +634,72 @@
             " locations."
         )
 
     if not built_locations:
         ui.print("No locations to deploy")
         return
 
+    try:
+        _deploy(
+            url=built_locations[0].url,
+            api_token=os.environ[TOKEN_ENV_VAR_NAME],
+            built_locations=built_locations,
+            location_load_timeout=location_load_timeout,
+            agent_heartbeat_timeout=agent_heartbeat_timeout,
+        )
+    except:
+        # unfortunately we do not know if only a subset of locations failed to deploy
+        for location_state in built_locations:
+            location_state.add_status_change(state.LocationStatus.failed, "deploy failed")
+            state_store.save(location_state)
+        raise
+    else:
+        for location_state in built_locations:
+            location_state.add_status_change(state.LocationStatus.success, "deploy successful")
+            state_store.save(location_state)
+
+    deployment_url = built_locations[0].url + "/" + built_locations[0].deployment_name
+    ui.print(f"View the status of your locations at {deployment_url}/locations.")
+
+
+@metrics.instrument(CliEventType.DEPLOY, tags=[CliEventTags.subcommand.dagster_cloud_ci])
+# url and api_token are used by the instrument decorator
+def _deploy(
+    *,
+    url: str,
+    api_token: str,
+    built_locations: List[state.LocationState],
+    location_load_timeout: int,
+    agent_heartbeat_timeout: int,
+):
     for location_state in built_locations:
         if not location_state.build_output:  # not necessary but keep type checker happy
             continue
 
         location_args = {
             "image": location_state.build_output.image,
             "location_file": location_state.location_file,
             "git_url": location_state.build.git_url,
             "commit_hash": location_state.build.commit_hash,
         }
         if location_state.build_output.strategy == "python-executable":
+            metrics.instrument_add_tags([CliEventTags.server_strategy.pex])
             location_args["pex_tag"] = location_state.build_output.pex_tag
+        else:
+            metrics.instrument_add_tags([CliEventTags.server_strategy.docker])
+
         with utils.client_from_env(location_state.url, location_state.deployment_name) as client:
             location_document = get_location_document(location_state.location_name, location_args)
             gql.add_or_update_code_location(client, location_document)
             ui.print(f"Updated code location {location_state.location_name} in dagster-cloud")
 
-    url = built_locations[0].url + "/" + built_locations[0].deployment_name
+    deployment_url = built_locations[0].url + "/" + built_locations[0].deployment_name
     with utils.client_from_env(
         built_locations[0].url, deployment=built_locations[0].deployment_name
     ) as client:
-        try:
-            wait_for_load(
-                client,
-                [location.location_name for location in built_locations],
-                location_load_timeout=location_load_timeout,
-                agent_heartbeat_timeout=agent_heartbeat_timeout,
-                url=url,
-            )
-        except:
-            # unfortunately we do not know if only a subset of locations failed to deploy
-            for location_state in built_locations:
-                location_state.add_status_change(state.LocationStatus.failed, "deploy failed")
-                state_store.save(location_state)
-            raise
-        else:
-            for location_state in built_locations:
-                location_state.add_status_change(state.LocationStatus.success, "deploy successful")
-                state_store.save(location_state)
-
-    ui.print(f"View the status of your locations at {url}/locations.")
+        wait_for_load(
+            client,
+            [location.location_name for location in built_locations],
+            location_load_timeout=location_load_timeout,
+            agent_heartbeat_timeout=agent_heartbeat_timeout,
+            url=deployment_url,
+        )
```

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/ci/checks.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/ci/checks.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/ci/report.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/ci/report.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/ci/state.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/ci/state.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/config.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/deployment/__init__.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/deployment/alert_policies/commands.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/deployment/alert_policies/commands.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/job/__init__.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/job/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/metrics.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/metrics.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/organization/__init__.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/organization/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/organization/saml/commands.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/organization/saml/commands.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/run/__init__.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/run/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/serverless/Dockerfile` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/serverless/Dockerfile`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/serverless/__init__.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/serverless/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,15 +73,18 @@
     ),
 }
 
 
 @app.command(name="build", short_help="Build image for Dagster Cloud code location.", hidden=True)
 @dagster_cloud_options(allow_empty=True, requires_url=True)
 @add_options(_BUILD_OPTIONS)
-@metrics.instrument(CliEventType.BUILD, tags=[CliEventTags.server_strategy.docker])
+@metrics.instrument(
+    CliEventType.BUILD,
+    tags=[CliEventTags.subcommand.dagster_cloud_serverless, CliEventTags.server_strategy.docker],
+)
 def build_command(
     api_token: str,
     url: str,
     location_load_timeout: int,
     agent_heartbeat_timeout: int,
     image: str = Argument(None, help="Image name."),
     **kwargs,
@@ -107,15 +110,18 @@
 
 @app.command(
     name="upload",
     short_help="Upload the built code location image to Dagster Cloud's image repository.",
     hidden=True,
 )
 @dagster_cloud_options(allow_empty=True, requires_url=True)
-@metrics.instrument(CliEventType.UPLOAD, tags=[CliEventTags.server_strategy.docker])
+@metrics.instrument(
+    CliEventType.UPLOAD,
+    tags=[CliEventTags.subcommand.dagster_cloud_serverless, CliEventTags.server_strategy.docker],
+)
 def upload_command(
     api_token: str,
     url: str,
     location_load_timeout: int,
     agent_heartbeat_timeout: int,
     image: str = Argument(None, help="Image name."),
     **kwargs,
@@ -177,15 +183,18 @@
         "Add a code location from a local directory, deployed as a Docker image. "
         "Also see 'deploy-python-executable' as an alternative deployment method."
     ),
 )
 @dagster_cloud_options(allow_empty=True, requires_url=True)
 @add_options(DEPLOY_DOCKER_OPTIONS)
 @add_options(DEPLOYMENT_CLI_OPTIONS)
-@metrics.instrument(CliEventType.DEPLOY, tags=[CliEventTags.server_strategy.docker])
+@metrics.instrument(
+    CliEventType.DEPLOY,
+    tags=[CliEventTags.subcommand.dagster_cloud_serverless, CliEventTags.server_strategy.docker],
+)
 def deploy_command(
     api_token: str,
     url: str,
     location_load_timeout: int,
     agent_heartbeat_timeout: int,
     deployment: str,
     source_directory: Path = Argument(".", help="Source directory."),
@@ -247,15 +256,18 @@
     name="upload-base-image",
     short_help=(
         "Upload a local Docker image to Dagster cloud, to use as a custom base image for"
         " deploy-python-executable."
     ),
 )
 @dagster_cloud_options(allow_empty=True, requires_url=True)
-@metrics.instrument(CliEventType.UPLOAD, tags=[CliEventTags.server_strategy.pex])
+@metrics.instrument(
+    CliEventType.UPLOAD,
+    tags=[CliEventTags.subcommand.dagster_cloud_serverless, CliEventTags.server_strategy.pex],
+)
 def upload_base_image_command(
     api_token: str,
     url: str,
     local_image: str = Argument(..., help="Pre-built local image, eg. 'local-image:local-tag'"),
     published_tag: str = Option(
         None,
         help=(
@@ -315,15 +327,18 @@
         "build_method": (
             pex_builder.deps.BuildMethod,
             Option("docker-fallback", help="Environment used to build the dependencies."),
         ),
     }
 )
 @dagster_cloud_options(allow_empty=True, requires_url=True)
-@metrics.instrument(CliEventType.BUILD, tags=[CliEventTags.server_strategy.pex])
+@metrics.instrument(
+    CliEventType.BUILD,
+    tags=[CliEventTags.subcommand.dagster_cloud_serverless, CliEventTags.server_strategy.pex],
+)
 def build_python_executable_command(
     code_directory: str,
     output_directory: str,
     python_version: str,
     build_method: pex_builder.deps.BuildMethod,
     api_token: str,
     url: str,
@@ -389,15 +404,18 @@
         "[Fast Deploys] Add a code location from a local directory, deployed as a Python"
         " executable. Also see 'deploy-docker' as an alternative deployment method."
     ),
 )
 @dagster_cloud_options(allow_empty=True, requires_url=True)
 @add_options(pex_utils.DEPLOY_PEX_OPTIONS)
 @add_options(DEPLOYMENT_CLI_OPTIONS)
-@metrics.instrument(CliEventType.DEPLOY, tags=[CliEventTags.server_strategy.pex])
+@metrics.instrument(
+    CliEventType.DEPLOY,
+    tags=[CliEventTags.subcommand.dagster_cloud_serverless, CliEventTags.server_strategy.pex],
+)
 def deploy_python_executable_command(
     api_token: str,
     url: str,
     location_load_timeout: int,
     agent_heartbeat_timeout: int,
     build_method: pex_builder.deps.BuildMethod,
     source_directory: Path = Argument(".", help="Source directory."),
```

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/commands/workspace/__init__.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/commands/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/config_utils.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/config_utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/docker_runner.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/docker_runner.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/errors.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/errors.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/graphql_client.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/graphql_client.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/headers/impl.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/headers/impl.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/code_location.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/pex_builder/code_location.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/deploy.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/pex_builder/deploy.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/deps.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/pex_builder/deps.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/git_context.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/pex_builder/git_context.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/github_context.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/pex_builder/github_context.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/gitlab_context.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/pex_builder/gitlab_context.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/parse_workspace.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/pex_builder/parse_workspace.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/pex_registry.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/pex_builder/pex_registry.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/selftest.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/pex_builder/selftest.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/source.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/pex_builder/source.py`

 * *Files 11% similar despite different names*

```diff
@@ -99,14 +99,18 @@
         init_file.write("# Auto generated package containing the original source at root/")
 
     shutil.copytree(
         code_directory,
         os.path.join(package_dir, "root"),
         dirs_exist_ok=True,
         ignore=shutil.ignore_patterns(*IGNORED_PATTERNS),
+        # We copy over symlinks as symlinks rather than try and resolve them and copy the target.
+        # This prevents build failures if the target file doesn't exist locally. If the target
+        # doesn't exist at runtime, this will fail and that is acceptable.
+        symlinks=True,
     )
 
 
 @click.command()
 @click.argument("project_dir", type=click.Path(exists=True))
 @click.argument("build_output_dir", type=click.Path(exists=False))
 @util.python_version_option()
```

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pex_builder/util.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/pex_builder/util.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/pydantic_yaml.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/pydantic_yaml.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/core/workspace.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/core/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/docker_utils.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/entrypoint.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/gql.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/gql.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/pex_utils.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/pex_utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/types.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -49,7 +49,11 @@
             "github",
             "gitlab",
             "jenkins",
             "travis",
             "unknown",
         ],
     )
+    subcommand = tags(
+        "subcommand",
+        ["dagster-cloud-ci", "dagster-cloud-serverless"],
+    )
```

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/ui.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/ui.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli/utils.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli.egg-info/SOURCES.txt` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli_tests/test_check.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli_tests/test_check.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli_tests/test_ci_commands.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli_tests/test_ci_commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -200,21 +200,23 @@
     monkeypatch.setenv("DAGSTER_CLOUD_API_TOKEN", "fake-token")
     mocker.patch(
         "dagster_cloud_cli.commands.ci.utils.get_registry_info",
         return_value={"registry_url": "example.com/image-registry"},
     )
     build_image = mocker.patch("dagster_cloud_cli.docker_utils.build_image", return_value=0)
     upload_image = mocker.patch("dagster_cloud_cli.docker_utils.upload_image", return_value=0)
+    mark_cli_event = mocker.patch("dagster_cloud_cli.gql.mark_cli_event", return_value=True)
 
     initialized_runner.invoke(app, ["ci", "locations-deselect", "a"])
     result = initialized_runner.invoke(app, ["ci", "build"])
     assert not result.exit_code, result.output
 
     assert len(build_image.call_args_list) == 2
     assert len(upload_image.call_args_list) == 2
+    assert len(mark_cli_event.call_args_list) == 2
 
     (b_build_dir, b_tag, b_registry_info), b_kwargs = build_image.call_args_list[0]
     (b_upload_tag, b_upload_registry_info), _ = upload_image.call_args_list[0]
     assert b_build_dir == "."
     assert b_tag.startswith(f"{deployment_name}-b")
     assert b_registry_info["registry_url"] == "example.com/image-registry"
     assert b_kwargs["base_image"] == "python:3.8-slim"
@@ -256,25 +258,27 @@
         "dagster_cloud_cli.commands.ci.utils.get_registry_info",
         return_value={"registry_url": "example.com/image-registry"},
     )
     mocker.patch("dagster_cloud_cli.docker_utils.build_image", return_value=0)
     mocker.patch("dagster_cloud_cli.docker_utils.upload_image", return_value=0)
     update_code_location = mocker.patch("dagster_cloud_cli.gql.add_or_update_code_location")
     wait_for_load = mocker.patch("dagster_cloud_cli.commands.ci.wait_for_load")
+    mark_cli_event = mocker.patch("dagster_cloud_cli.gql.mark_cli_event", return_value=True)
 
     initialized_runner.invoke(app, ["ci", "locations-deselect", "a"])
     result = initialized_runner.invoke(app, ["ci", "build"])
     assert not result.exit_code, result.output
     print(result.output)
     result = initialized_runner.invoke(app, ["ci", "deploy"])
     assert not result.exit_code, result.output
     print(result.output)
 
     assert len(update_code_location.call_args_list) == 2
     assert len(wait_for_load.call_args_list) == 1
+    assert len(mark_cli_event.call_args_list) == 3  # 2 for building 2 locations, 1 for deploy
 
     (gql_shim, b_update_args), _ = update_code_location.call_args_list[0]
     (_, c_update_args), _ = update_code_location.call_args_list[1]
     assert b_update_args == {
         "code_source": {"module_name": "b"},
         "git": {"commit_hash": "hash-4354"},
         "image": f"example.com/image-registry:{deployment_name}-b-hash-4354",
@@ -288,14 +292,23 @@
         "location_name": "c",
         "working_directory": "c",
     }
     (_, wait_location_args), wait_kwargs = wait_for_load.call_args_list[0]
     assert wait_location_args == ["b", "c"]
     assert wait_kwargs["url"] == f"https://some-org.dagster.cloud/{deployment_name}"
 
+    assert [call_kwarg["event_type"].name for (_, call_kwarg) in mark_cli_event.call_args_list] == [
+        "BUILD",
+        "BUILD",
+        "DEPLOY",
+    ]
+
+    for _, call_kwarg in mark_cli_event.call_args_list:
+        assert "subcommand:dagster-cloud-ci" in call_kwarg["tags"]
+
     # first location (a) is deselected
     assert [
         location["history"][-1]["status"] for location in get_locations(initialized_runner)
     ] == ["pending", "success", "success"]
 
 
 def test_ci_set_build_output(initialized_runner: CliRunner):
```

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli_tests/test_gql.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli_tests/test_gql.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud_cli-1.3.5/dagster_cloud_cli_tests/test_metrics.py` & `dagster_cloud_cli-1.3.6/dagster_cloud_cli_tests/test_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,9 +240,11 @@
                 # We cast the url to a string but we want to make sure
                 # the original url isn't None
 
                 # If this test fails, it's usually because the instrument
                 # decorator is in the wrong place.
                 url = gql.graphql_client_from_url.call_args_list[0].kwargs.get("url")
                 assert "None" not in url, f"Command {command} wasn't provided a url"
+                gql.mark_cli_event.reset_mock()
+                gql.graphql_client_from_url.reset_mock()
 
     walk_cli(app)
```

### Comparing `dagster_cloud_cli-1.3.5/setup.py` & `dagster_cloud_cli-1.3.6/setup.py`

 * *Files identical despite different names*

